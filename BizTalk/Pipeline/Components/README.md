# Be.Stateless.BizTalk.Pipeline.Components

<div class="badges">
<div>

[![][github.badge]][github]

[![][release.badge]][release]

</div>
<div>

[![][pipeline.ci.badge]][pipeline.ci]

[![][pipeline.mr.badge]][pipeline.mr]

</div>
<div>

[![][nuget.badge]][nuget]

[![][nuget.unit.badge]][nuget.unit]

[![][nuget.nunit.badge]][nuget.nunit]

[![][nuget.xunit.badge]][nuget.xunit]

</div>
</div>

## Overview

`Be.Stateless.BizTalk.Pipeline.Components` is part of the [BizTalk.Factory Application](./../../Factory/Application/README.md) Package. This component provides very lightweight yet tremendously helpful Microsoft BizTalk Server® pipeline components. It is accompanied by a set of unit-testing helper components meant to support the developer in writing custom pipeline components and their unit tests.

## Be.Stateless.BizTalk.Pipeline.Components

All this component provides are 3 seemingly insignificant classes:

- [Be.Stateless.BizTalk.Component.PipelineComponent][pipeline-component], which is a base class for developing custom Microsoft BizTalk Server® pipeline components that takes care of all the mundane and routine code that any pipeline component must implement: primarily loading and saving configuration state, error handling and logging but also `Name`, `Description`, `Icon`, and all other required low-value properties and methods. In addition, it provides support for a pipeline component to be disabled &mdash;through the `Enabled` property&mdash; and its execution being skipped while the pipeline is processing the messages passing through;

- [Be.Stateless.BizTalk.Component.FailedMessageRoutingEnablerComponent][failed-message-routing-enabler-component], which is a pipeline component that enables routing of failed messages &mdash;similarly to what can be done through configuration via the Microsoft BizTalk Server® administration console for instance&mdash; and prevents routing failure reports from being generated &mdash;what can only be done by code and not through configuration;

- [Be.Stateless.BizTalk.Component.MicroPipelineComponent][micro-pipeline-component], which is a pipeline component acting as a micro runtime allowing to run a series of configurable micro components &mdash;i.e. components implementing [Be.Stateless.BizTalk.MicroComponent.IMicroComponent][i-micro-component],&mdash; similarly to what a regular Microsoft BizTalk Server® pipeline would do if the micro components were regular pipeline components.

> **Remark** `Be.Stateless.BizTalk.Pipeline.Components` component is part of the `BizTalk.Factory Application`, which is deployed as a full-fledged Microsoft BizTalk Server® application, and it cannot consequently be redeployed without first unenlisting or undeploying any other Microsoft BizTalk Server® applications that depends on it. That would inevitably lead to downtime and operational overheads, but due to their very generic or mediating implementations, these pipeline components should never require a complete redeployment &mdash;at worst, a new GAC deployment on rare occasions.

### Using and Configuring the `MicroPipelineComponent`

Besides the fact that, thanks to `MicroPipelineComponent`, developers no longer need to constantly define and deploy custom Microsoft BizTalk Server® pipelines, what the real added value this pipeline component brings forward is that it can easily be **entirely reconfigured** without any downtime nor any deployment or administrative restriction. Noticeably, extending, rearranging, or reducing the series of micro components that a given `MicroPipelineComponent` instance will run can trivially be accomplished through the Microsoft BizTalk Server® administration console, what is impossible to achieve with traditional Microsoft BizTalk Server® pipelines.

That being said, coming with the right value to feed to the `MicroPipelineComponent`'s `Components` property, which is of type `IEnumerable<IMicroComponent>`, through the Microsoft BizTalk Server® administration console might not be trivial. Internally, this property serializes itself as an `XML` string that encompasses the `XML` serialization of its micro components; see the following example. Notice also that to feed this `XML` string through the Microsoft BizTalk Server® administration console, it must be a one liner!

```xml
<mComponents>
    <mComponent name='Be.Stateless.BizTalk.MicroComponent.ContextPropertyExtractor, Be.Stateless.BizTalk.Pipeline.MicroComponents, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14'>
        <Extractors />
    </mComponent>
    <mComponent name='Be.Stateless.BizTalk.MicroComponent.ContextBuilder, Be.Stateless.BizTalk.Pipeline.MicroComponents, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14'>
        <Builder>Be.Stateless.BizTalk.Dummies.Bindings.DummyContextBuilder, Be.Stateless.BizTalk.Dsl.Binding.Dummies, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14</Builder>
        <ExecutionTime>Deferred</ExecutionTime>
    </mComponent>
    <mComponent name='Be.Stateless.BizTalk.MicroComponent.ActivityTracker, Be.Stateless.BizTalk.Activity.Tracking, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14'>
        <TrackingContextCacheDuration>00:01:00</TrackingContextCacheDuration>
        <TrackingModes>Context</TrackingModes>
    </mComponent>
    <mComponent name='Be.Stateless.BizTalk.MicroComponent.XmlTranslator, Be.Stateless.BizTalk.Pipeline.MicroComponents, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14'>
        <Encoding>utf-8</Encoding>
        <Modes>Default</Modes>
        <Translations override='false'>
            <NamespaceTranslation matchingPattern='.*' replacementPattern='urn:schemas.stateless.be:biztalk:claim:2017:04'
                xmlns='urn:schemas.stateless.be:biztalk:translations:2013:07' />
            <NamespaceTranslation matchingPattern='^urn:dummy:2021:11:11$' replacementPattern='urn:schemas.stateless.be:biztalk:claim:2017:04'
                xmlns='urn:schemas.stateless.be:biztalk:translations:2013:07' />
        </Translations>
    </mComponent>
</mComponents>
```

If developers had to manually craft these `XML` by hand, the use of the `MicroPipelineComponent` pipeline component would be subject to a severe impairment. To circumvent this issue, `BizTalk.Factory` comes with a `C#` embedded [DSL][dsl] that allows developers to write the previous configuration entirely in a type safe `C#` way, as the following excerpt demonstrates:

```csharp
... new ReceivePipeline<PassThruReceive>(pl => pl.Decoder<MicroPipelineComponent>(c => {
    c.Components = new IMicroComponent[] {
        new ContextPropertyExtractor(),
        new ContextBuilder {
            ExecutionTime = PluginExecutionTime.Deferred,
            BuilderType = typeof(DummyContextBuilder)
        },
        new ActivityTracker {
            TrackingModes = ActivityTrackingModes.Context
        },
        new XmlTranslator {
            Translations = new() { Items = new XmlNamespaceTranslation[] {
                new() {
                    MatchingPatternString = ".*",
                    ReplacementPattern = SchemaMetadata.For<Claim.CheckOut>().TargetNamespace
                },
                new() {
                    MatchingPatternString = "^urn:dummy:2021:11:11$",
                    ReplacementPattern = SchemaMetadata.For<Claim.CheckIn>().TargetNamespace
                }
            }}
        }
    };
}));
```

Notice that this code is what is actually used at deployment time by `BizTalk.Factory` to generate the Microsoft BizTalk Server® `XML` application bindings to import. For further explanation, the developer is invited to browse the documentation and features offered by [Be.Stateless.BizTalk.Dsl.Binding](./../../Dsl/Binding/README.md) and [Be.Stateless.BizTalk.Dsl.Pipeline](./../../Dsl/Pipeline/README.md).

> **Remark** Out of the box, `BizTalk.Factory` provides a versatile set of pipelines hosting this `MicroPipelineComponent` pipeline component, see [Be.Stateless.BizTalk.Pipelines](./../../Pipelines/README.md), as well as a bunch of reusable micro components providing a whole wealth of services, see [Be.Stateless.BizTalk.MicroComponents](./../MicroComponents/README.md).

### `MicroPipelineComponent` Implementation

It is worth noticing that `MicroPipelineComponent` itself delegates its implementation to a pseudo &mdash;because it does not implement the `IMicroComponent` interface&mdash; micro component, i.e. [MicroPipeline][micro-pipeline], that comes with the same GAC-only deployment constraints as all the components being part of the [`BizTalk.Factory` Runtime Package](./../../Factory/Runtime/README.md). Even the serialization of the micro components declared at the `MicroPipelineComponent` level is taken care of by the pseudo micro component [MicroPipeline][micro-pipeline]; it would therefore be possible, for instance, to change the serialization format from `XML` to anything else without any deployment impact on Microsoft BizTalk Server® other than a reconfiguration of the pipelines of all the receiving locations and sending ports defined in Microsoft BizTalk Server® that depend on the `MicroPipelineComponent` pipeline component.

## Developing and Testing Custom Pipeline Components

1. Be.Stateless.BizTalk.Pipeline.Components.Unit
2. Be.Stateless.BizTalk.Pipeline.Components.NUnit
3. Be.Stateless.BizTalk.Pipeline.Components.XUnit

<!-- TODO -->

<!-- links -->

[github]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.Components "Be.Stateless.BizTalk.Pipeline.Components GitHub Repository"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.BizTalk.Pipeline.Components&logo=github
[nuget]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Pipeline.Components "Be.Stateless.BizTalk.Pipeline.Components NuGet Package"
[nuget.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Pipeline.Components.svg?label=Be.Stateless.BizTalk.Pipeline.Components&style=flat?style=plastic&logo=nuget
[nuget.unit]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Pipeline.Components.Unit "Be.Stateless.BizTalk.Pipeline.Components.Unit NuGet Package"
[nuget.unit.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Pipeline.Components.Unit.svg?label=Be.Stateless.BizTalk.Pipeline.Components.Unit&style=flat&logo=nuget
[nuget.nunit]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Pipeline.Components.NUnit "Be.Stateless.BizTalk.Pipeline.Components.NUnit NuGet Package"
[nuget.nunit.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Pipeline.Components.NUnit.svg?label=Be.Stateless.BizTalk.Pipeline.Components.NUnit&style=flat&logo=nuget
[nuget.xunit]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Pipeline.Components.XUnit "Be.Stateless.BizTalk.Pipeline.Components.XUnit NuGet Package"
[nuget.xunit.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Pipeline.Components.XUnit.svg?label=Be.Stateless.BizTalk.Pipeline.Components.XUnit&style=flat&logo=nuget
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=37&branchName=master "Azure DevOps Continuous Integration Build Pipeline"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Pipeline.Components%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=38&branchName=master "Azure DevOps Release Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Pipeline.Components%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[release]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.Components/releases/latest "Be.Stateless.BizTalk.Pipeline.Components Release"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.Pipeline.Components?label=Release&logo=github
[dsl]: https://en.wikipedia.org/wiki/Domain-specific_language "Domain-Specific Language"
[failed-message-routing-enabler-component]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.Components/blob/master/src/Be.Stateless.BizTalk.Pipeline.Components/Component/FailedMessageRoutingEnablerComponent.cs
[i-micro-component]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/IMicroComponent.cs
[micro-pipeline]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/MicroPipeline.cs
[micro-pipeline-component]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.Components/blob/master/src/Be.Stateless.BizTalk.Pipeline.Components/Component/MicroPipelineComponent.cs
[pipeline-component]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.Components/blob/master/src/Be.Stateless.BizTalk.Pipeline.Components/Component/PipelineComponent.cs

<!--
cSpell:ignore biztalk typeof undeploying unenlisting
-->
