# Pipeline Binding

> **Downloads** The code samples used in this user guide have been made available in the [Be.Stateless.BizTalk.Factory.Samples][github.samples] GitHub repository.

Let us configure the pipelines for our sample Microsoft BizTalk Server® [Receive Locations](./ReceiveLocation.md) and [Send Ports](./SendPort.md). Depending on whether the location or port should be a one-way or two-way [Message Endpoint][message-endpoint], the developer will have to add either a single receive or send pipeline, or both.

## Receive Pipeline Binding

We left off our sample `Credit Note Receive Location` in a state where the `ApplicationFixture` is failing because the _"[Credit Note Receive Location] Receive Location's Receive Pipeline is not defined."_.

In order to be able to add a receive pipeline to our receive location, we need to add a reference to the assembly containing the pipeline we need. Let us reference to the `Be.Stateless.BizTalk.Pipelines` `NuGet` package from the `Org.Anization.Accounting.Bindings` project and configure our receive location's receive pipeline.

> **Remark** In order to be configure a pipeline, we cannot simply new it and assign it to our receive location or send port; we instead need an API allowing us to configure any of its constituting pipeline components, whatever their pipeline stage, in a `C#` type-safe way. `Be.Stateless.BizTalk.Dsl.Binding` provides two generic helper classes that allow us to tap into the configuration of the pipelines and its components:
>
> - [Be.Stateless.BizTalk.Dsl.Binding.ReceivePipeline\<T>][receive-pipeline-of-t]
>
> - [Be.Stateless.BizTalk.Dsl.Binding.SendPipeline\<T>][send-pipeline-of-t]
>
> Notice that `T` is the actual runtime pipeline type and not its [Be.Stateless.BizTalk.Dsl.Pipeline](./../Pipeline/README.md) definition type; one can therefore configure any actual Microsoft BizTalk Server® pipeline without restrictions.

```csharp
using Be.Stateless.BizTalk.MicroPipelines;

...
ReceiveLocation(
  rl => {
    rl.Name = "Credit Note Receive Location";
    rl.ReceivePipeline = new ReceivePipeline<XmlReceive>();
})
...
```

Referencing the `Be.Stateless.BizTalk.Pipelines` `NuGet` package alone is however not enough as the project's compilation would fail, complaining that _The type 'ReceivePipeline' is defined in an assembly that is not referenced. You must add a reference to assembly 'Microsoft.BizTalk.Pipeline, Version=3.0.1.0, Culture=neutral, PublicKeyToken=31bf3856ad364e35'._ To remedy this issue, let us reference the `BizTalk.Server.2020.Runtime` `NuGet` package and run the unit tests once more.

Even though the compilation now succeeds, the unit test fails complaining that it _Did not expect any exception, but found System.IO.FileNotFoundException with message "Could not load file or assembly 'Microsoft.BizTalk.PipelineOM, Version=3.0.1.0, Culture=neutral, PublicKeyToken=31bf3856ad364e35' or one of its dependencies. The system cannot find the file specified."_ To remedy this issue, let us reference the same `BizTalk.Server.2020.Runtime` `NuGet` package from the `Org.Anization.Accounting.Bindings.Tests` project too and run the unit tests once again.

> **Remark** `BizTalk.Server.2020.Runtime` contains the Microsoft BizTalk Server® 2020 runtime assemblies, that is to say all the assemblies that are required to be both referenced at _development time_ and be available at _runtime_ &mdash;these are typically the assemblies that are deployed in the GAC.

The unit test still fails complaining now that it _Did not expect any exception, but found System.IO.FileNotFoundException with message "Could not load file or assembly 'PipelineObjects, Version=3.0.1.0, Culture=neutral, PublicKeyToken=31bf3856ad364e35' or one of its dependencies. The system cannot find the file specified."_ Let us reference the `BizTalk.Server.2020.Utilities` `NuGet` package from the `Org.Anization.Accounting.Bindings.Tests` project and run the unit tests one more time.

> **Remark** `BizTalk.Server.2020.Utilities` contains the Microsoft BizTalk Server® 2020 non-runtime assemblies, that is to say the assemblies that are only required to be referenced at development time but not to be available at runtime &mdash;these are typically the assemblies found in the `C:\Program Files (x86)\Microsoft BizTalk Server\Developer Tools` directory.

### Receive Pipeline Component Configuration

Configuring the components of a given pipeline obviously requires us to know what are its constituting components but `Be.Stateless.BizTalk.Dsl.Binding` has a lot of safety nets to prevent us from making stupid mistakes.

Let us try to configure the `Be.Stateless.BizTalk.MicroPipelines.XmlReceive` pipeline. We know that, for simplicity and efficiency's sake, all the micro pipelines &mdash;but the pass-thru ones, for obvious reasons&mdash; embed two `Be.Stateless.BizTalk.Component.MicroPipelineComponent`s, one before the assembling/disassembling stage and one after it. We also know that a receive pipeline has 4 stages &mdash;`Decode`, `Disassemble`, `Validate`, and `ResolveParty`.

> **Remark** `Be.Stateless.BizTalk.Dsl.Binding` API has been carefully crafted so as to provide a rich intellisense experience &mdash;as illustrated [here][receive-pipeline-intellisense]&mdash; that can even help you remember what are the various stages of a receive pipeline.

What receive pipeline's stage embeds the second `Be.Stateless.BizTalk.Component.MicroPipelineComponent`? Is it the `Validate` or the `ResolveParty` stage? As we are pretty confident this is the latter one, let us try to configure the receive pipeline of our `Credit Note Receive Location`.

```csharp
using Be.Stateless.BizTalk.Component;
using Be.Stateless.BizTalk.Dsl.Binding;
using Be.Stateless.BizTalk.MicroComponent;
using Be.Stateless.BizTalk.MicroPipelines;
using Be.Stateless.BizTalk.Schema;
using Microsoft.BizTalk.Component;
using Microsoft.BizTalk.Component.Utilities;

rl.ReceivePipeline = new ReceivePipeline<XmlReceive>(
  p => {
    p.Decoder<MicroPipelineComponent>(
      c => {
        c.Components = new IMicroComponent[] {
          new ContextBuilder { BuilderType = typeof(...) }
        };
      })
    .Disassembler<XmlDasmComp>(
      d => {
        d.DocumentSpecNames = new SchemaList {
          new SchemaWithNone(SchemaMetadata.For<Any>().DocumentSpec.DocSpecStrongName)
        };
      })
    .PartyResolver<MicroPipelineComponent>(
      c => {
        c.Components = new IMicroComponent[] {
          new XsltRunner { MapType = typeof(...) }
        };
      });
});
```

As usual, let us validate our configuration by running the unit tests. The `ApplicationFixture` fails this time complaining that it _Did not expect any exception, but found System.InvalidOperationException with message "Stage 'PartyResolver' has no 'MicroPipelineComponent' component."_ Well, we were wrong, the `Be.Stateless.BizTalk.Component.MicroPipelineComponent` does not belong to the `ResolveParty` stage; it must therefore belong to the `Validate` one. Let us fix the code.

```csharp
rl.ReceivePipeline = new ReceivePipeline<XmlReceive>(
  p => {
    ...
    .Disassembler<XmlDasmComp>(
      d => {
        ...
      })
    .Validator<MicroPipelineComponent>(
      c => {
        ...
      });
});
```

> **Remark** The `API` to configure a pipeline's components is actually provided together by `Be.Stateless.BizTalk.Dsl.Binding` and `Be.Stateless.BizTalk.Dsl.Pipeline`. The `API` to fetch a given [component][i-component-list] at a given [stage][i-stage] of either a [receive pipeline][i-receive-pipeline-stage-list] or a [send pipeline][i-send-pipeline-stage-list] is actually part of the `Pipeline DSL`, whose different alternate syntaxes are illustrated by the `Binding DSL` through the [ReceivePipelineDslGrammarVariant\*][receive-pipeline-dsl-grammar-variant] and [SendPipelineDslGrammarVariant\*][send-pipeline-dsl-grammar-variant] test methods.

For the sake of completeness, here is the configuration of the separate `BribeReceiveLocation` type, which is identical, `API` wise, to the one of the inline `Credit Note Receive Location`.

```csharp
public BribeReceiveLocation()
{
  Name = "Bribe Receive Location";
  ReceivePipeline = new ReceivePipeline<PassThruReceive>();
}
```

## Send Pipeline Binding

As illustrated below, configuring a send pipeline's binding for a port is very similar to configuring a [receive pipeline's binding](#receive-pipeline-binding):

```csharp
using Be.Stateless.BizTalk.MicroPipelines;

...
SendPort(
  sp => {
    sp.Name = "Embezzlement Send Port";
    sp.SendPipeline = new SendPipeline<XmlTransmit>();
})
...
```

> **Remark** The embedded C# DSL, being type-safe, naturally prevents the developer from mistakenly trying to configure a port's send pipeline via the [ReceivePipeline\<T>][receive-pipeline-of-t] configuration helper, or vice versa, a port's receive pipeline via the [SendPipeline\<T>][send-pipeline-of-t] configuration helper.

### Send Pipeline Component Configuration

Configuring the components of a send pipeline through the [SendPipeline\<T>][send-pipeline-of-t] generic configuration helper is similar to [configuring the components of a receive pipeline](#receive-pipeline-component-configuration) with the noticeable exception that a send pipeline has 3 different stages &mdash;`PreAssemble`, `Assemble`, and `Encode`.

> **Remark** `Be.Stateless.BizTalk.Dsl.Binding` API has been carefully crafted so as to provide a rich intellisense experience &mdash;as illustrated [here][send-pipeline-intellisense]&mdash; that can even help you remember what are the various stages of a send pipeline.

```csharp
using Be.Stateless.BizTalk.Component;
using Be.Stateless.BizTalk.Dsl.Binding;
using Be.Stateless.BizTalk.MicroComponent;
using Be.Stateless.BizTalk.MicroPipelines;
using Be.Stateless.BizTalk.Schema;
using Microsoft.BizTalk.Component;
using Microsoft.BizTalk.Component.Utilities;

sp.SendPipeline = new SendPipeline<FFTransmit>(
  p => {
    p.PreAssembler<MicroPipelineComponent>(
        c => {
          c.Components = new IMicroComponent[] {
            new XsltRunner { MapType = typeof(...) }
          };
        })
      .Assembler<FFAsmComp>(
        c => {
          c.HeaderSpecName = new SchemaWithNone(SchemaMetadata.For<...>().DocumentSpec.DocSpecStrongName);
          c.DocumentSpecName = new SchemaWithNone(SchemaMetadata.For<...>().DocumentSpec.DocSpecStrongName);
          c.TrailerSpecName = new SchemaWithNone(SchemaMetadata.For<...>().DocumentSpec.DocSpecStrongName);
        })
      .Encoder<MicroPipelineComponent>(
        c => {
          c.Components = new IMicroComponent[] {
            new ContextBuilder { BuilderType = typeof(...) }
          };
        });
  });

```

<!-- links -->

[github.samples]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples

<!--  -->

[i-component-list]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Pipeline/blob/master/src/Be.Stateless.BizTalk.Dsl.Pipeline/Dsl/Pipeline/IComponentList.cs
[i-receive-pipeline-stage-list]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Pipeline/blob/master/src/Be.Stateless.BizTalk.Dsl.Pipeline/Dsl/Pipeline/IReceivePipelineStageList.cs
[i-send-pipeline-stage-list]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Pipeline/blob/master/src/Be.Stateless.BizTalk.Dsl.Pipeline/Dsl/Pipeline/ISendPipelineStageList.cs
[i-stage]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Pipeline/blob/master/src/Be.Stateless.BizTalk.Dsl.Pipeline/Dsl/Pipeline/IStage.cs
[message-endpoint]: https://www.enterpriseintegrationpatterns.com/patterns/messaging/MessageEndpoint.html
[receive-pipeline-dsl-grammar-variant]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding.Tests/Dsl/Binding/Xml/Serialization/PipelineBindingInfoSerializerFixture.cs#L39
[receive-pipeline-intellisense]: ./../../../assets/images/ReceivePipeline.Intellisense.png
[receive-pipeline-of-t]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/ReceivePipeline.cs
[send-pipeline-dsl-grammar-variant]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding.Tests/Dsl/Binding/Xml/Serialization/PipelineBindingInfoSerializerFixture.cs#L345
[send-pipeline-intellisense]: ./../../../assets/images/SendPipeline.Intellisense.png
[send-pipeline-of-t]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/SendPipeline.cs

<!--
cSpell:ignore Anization Dasm typeof
-->
