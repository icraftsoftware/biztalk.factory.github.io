# Be.Stateless.BizTalk.Pipelines

[![][github.badge]][github]

##### Build Pipelines

[![][pipeline.mr.badge]][pipeline.mr]

[![][pipeline.ci.badge]][pipeline.ci]

##### Latest Release

[![][nuget.badge]][nuget]

[![][release.badge]][release]

##### Release Preview

[![][nuget.preview.badge]][nuget.preview]

## Overview

`Be.Stateless.BizTalk.Pipelines` is part of the [BizTalk.Factory Application](./../Factory/Application/README.md) Package. This component provides versatile _"one-size-fits-all"_ pipelines for general purpose Microsoft BizTalk Server® development.

## Be.Stateless.BizTalk.Pipelines

`Be.Stateless.BizTalk.Pipelines` provides three sets of Microsoft BizTalk Server® pipelines. Each set supports both inbound and outbound message processing and each set's purpose is determined by the component being hosted in the Assembling/Disassembling stage. Specifically, `BizTalk.Factory` provides the following pipelines:

- `Be.Stateless.BizTalk.MicroPipelines.FFReceive` which is used for scenarios where flat-file message payload processing is necessary upon receiving messages. It is defined as [follows][ff-receive];

- `Be.Stateless.BizTalk.MicroPipelines.FFTransmit` which is used for scenarios where flat-file message payload processing is necessary upon sending messages. It is defined as [follows][ff-transmit];

- `Be.Stateless.BizTalk.MicroPipelines.PassThruReceive` which is used for pass-through scenarios where no message payload processing is necessary upon receiving messages. It is defined as [follows][pass-thru-receive];

- `Be.Stateless.BizTalk.MicroPipelines.PassThruTransmit` which is used for pass-through scenarios where no message payload processing is necessary upon sending messages. It is defined as [follows][pass-thru-transmit];

- `Be.Stateless.BizTalk.MicroPipelines.XmlReceive` which is used for scenarios where `XML` message payload processing is necessary upon receiving messages. It is defined as [follows][xml-receive];

- `Be.Stateless.BizTalk.MicroPipelines.XmlTransmit` which is used for scenarios where `XML` message payload processing is necessary upon sending messages. It is defined as [follows][xml-transmit].

These pipelines have been dubbed **micro pipelines** because they essentially host up to two instances of the `MicroPipelineComponent` pipeline component &mdash;see [Be.Stateless.BizTalk.Pipeline.Components](./../Pipeline/Components/README.md) for further information,&mdash; one before and one after the assembler/disassembler component if it is present or just a single one if no assembler/disassembler component is present. In a given pipeline, the `MicroPipelineComponent` is obviously repeated to provide maximum configuration flexibility.

## Pipeline Definitions

It is worth noticing that these pipelines have not been defined via the Microsoft BizTalk Server® designer surface but have been directly defined in a `C#` type-safe way thanks to a `C#` embedded DSL, [Be.Stateless.BizTalk.Dsl.Pipeline](./../Dsl/Pipeline/README.md), tailored for pipelines. All their definitions can be found in the `Be.Stateless.BizTalk.Pipeline.Definitions` project in the same [GitHub][github] repository.

## Pipeline Build

Just because it references the `Be.Stateless.BizTalk.Pipeline.Definitions` project, the `Be.Stateless.BizTalk.Pipelines` project will produce pipeline designer surface equivalent outputs when being built. This is made possible thanks to the conjunctive work of both the [BizTalk.Server.2020.Build](./../Build/Tasks/README.md) and [Be.Stateless.BizTalk.Build.Tasks](./../Build/Tasks/README.md) components to process the pipeline definitions found in the referenced `Be.Stateless.BizTalk.Pipeline.Definitions` project.

All the pipeline designer surface equivalent outputs, i.e. the `*.btp` files, can be found in the `Be.Stateless.BizTalk.Pipelines` project in the same [GitHub][github] repository. Notice that these files are being generated anew at each build; they have been committed into the source code for simplicity's sake.

For illustration's sake, here is the `C#` definition of the `Be.Stateless.BizTalk.MicroPipelines.XmlReceive`:

```csharp
public class XmlReceive : ReceivePipeline
{
  public XmlReceive()
  {
    Description = "XML receive micro-pipeline.";
    Version = new(1, 0);
    Stages.Decode
      .AddComponent(new FailedMessageRoutingEnablerComponent())
      .AddComponent(new MicroPipelineComponent { Enabled = true });
    Stages.Disassemble
      .AddComponent(new XmlDasmComp());
    Stages.Validate
      .AddComponent(new MicroPipelineComponent { Enabled = true });
  }
}
```

And its designer-surface equivalent `.btp` output file:

```xml
<Document xmlns:xsi='http://www.w3.org/2001/XMLSchema-instance' xmlns:xsd='http://www.w3.org/2001/XMLSchema' PolicyFilePath='BTSReceivePolicy.xml' MajorVersion='1' MinorVersion='0'>
  <Description>XML receive micro-pipeline.</Description>
  <Stages>
    <Stage CategoryId='9d0e4103-4cce-4536-83fa-4a5040674ad6'>
      <Components>
        <Component>
          <Name>Be.Stateless.BizTalk.Component.FailedMessageRoutingEnablerComponent</Name>
          <ComponentName>FailedMessageRoutingEnablerComponent</ComponentName>
          <Description>Enables routing of failed messages and prevents routing failure reports from being generated.</Description>
          <Version>2.0</Version>
          <Properties>
            <Property Name='Enabled'>
              <Value xsi:type='xsd:boolean'>true</Value>
            </Property>
            <Property Name='EnableFailedMessageRouting'>
              <Value xsi:type='xsd:boolean'>true</Value>
            </Property>
            <Property Name='SuppressRoutingFailureReport'>
              <Value xsi:type='xsd:boolean'>true</Value>
            </Property>
          </Properties>
          <CachedDisplayName>FailedMessageRoutingEnablerComponent</CachedDisplayName>
          <CachedIsManaged>true</CachedIsManaged>
        </Component>
        <Component>
          <Name>Be.Stateless.BizTalk.Component.MicroPipelineComponent</Name>
          <ComponentName>MicroPipelineComponent</ComponentName>
          <Description>Runs a sequence of micro components as if they were regular pipeline components.</Description>
          <Version>2.0</Version>
          <Properties>
            <Property Name='Enabled'>
              <Value xsi:type='xsd:boolean'>true</Value>
            </Property>
            <Property Name='Components'>
              <Value xsi:type='xsd:string' />
            </Property>
          </Properties>
          <CachedDisplayName>MicroPipelineComponent</CachedDisplayName>
          <CachedIsManaged>true</CachedIsManaged>
        </Component>
      </Components>
    </Stage>
    <Stage CategoryId='9d0e4105-4cce-4536-83fa-4a5040674ad6'>
      <Components>
        <Component>
          <Name>Microsoft.BizTalk.Component.XmlDasmComp</Name>
          <ComponentName>XML disassembler</ComponentName>
          <Description>Streaming XML disassembler</Description>
          <Version>1.0</Version>
          <Properties>
            <Property Name='EnvelopeSpecNames'>
              <Value xsi:type='xsd:string' />
            </Property>
            <Property Name='EnvelopeSpecTargetNamespaces'>
              <Value xsi:type='xsd:string' />
            </Property>
            <Property Name='DocumentSpecNames'>
              <Value xsi:type='xsd:string' />
            </Property>
            <Property Name='DocumentSpecTargetNamespaces'>
              <Value xsi:type='xsd:string' />
            </Property>
            <Property Name='AllowUnrecognizedMessage'>
              <Value xsi:type='xsd:boolean'>false</Value>
            </Property>
            <Property Name='ValidateDocument'>
              <Value xsi:type='xsd:boolean'>false</Value>
            </Property>
            <Property Name='RecoverableInterchangeProcessing'>
              <Value xsi:type='xsd:boolean'>false</Value>
            </Property>
            <Property Name='HiddenProperties'>
              <Value xsi:type='xsd:string'>EnvelopeSpecTargetNamespaces,DocumentSpecTargetNamespaces</Value>
            </Property>
            <Property Name='DtdProcessing'>
              <Value xsi:type='xsd:string' />
            </Property>
          </Properties>
          <CachedDisplayName>XML disassembler</CachedDisplayName>
          <CachedIsManaged>true</CachedIsManaged>
        </Component>
      </Components>
    </Stage>
    <Stage CategoryId='9d0e410d-4cce-4536-83fa-4a5040674ad6'>
      <Components>
        <Component>
          <Name>Be.Stateless.BizTalk.Component.MicroPipelineComponent</Name>
          <ComponentName>MicroPipelineComponent</ComponentName>
          <Description>Runs a sequence of micro components as if they were regular pipeline components.</Description>
          <Version>2.0</Version>
          <Properties>
            <Property Name='Enabled'>
              <Value xsi:type='xsd:boolean'>true</Value>
            </Property>
            <Property Name='Components'>
              <Value xsi:type='xsd:string' />
            </Property>
          </Properties>
          <CachedDisplayName>MicroPipelineComponent</CachedDisplayName>
          <CachedIsManaged>true</CachedIsManaged>
        </Component>
      </Components>
    </Stage>
    <Stage CategoryId='9d0e410e-4cce-4536-83fa-4a5040674ad6'>
      <Components />
    </Stage>
  </Stages>
</Document>
```

Which displays as follows when opened in the designer surface:

![XmlReceive][xml-receive.btp]

For the sake of completeness, [Be.Stateless.BizTalk.Build.Tasks](./../Build/Tasks/README.md), with the help of [BizTalk.Server.2020.Build](./../Build/Tasks/README.md), substitutes itself to the default Microsoft BizTalk Server® pipeline compiler and produces the following `.btp.cs` output file &mdash;the astute reader will immediately notice how much more readable, explicit and better formatted this code is in comparison with the one produced by the default compiler:

```csharp
namespace Be.Stateless.BizTalk.MicroPipelines
{
  public sealed class XmlReceive : Microsoft.BizTalk.PipelineOM.ReceivePipeline
  {
    public XmlReceive()
    {
      Microsoft.BizTalk.PipelineOM.Stage stage = this.AddStage(Microsoft.BizTalk.PipelineOM.Stage.Decoder, Microsoft.BizTalk.PipelineOM.ExecutionMode.all);
      Microsoft.BizTalk.Component.Interop.IBaseComponent comp0 = Microsoft.BizTalk.PipelineOM.PipelineManager.CreateComponent("Be.Stateless.BizTalk.Component.FailedMessageRoutingEnablerComponent, Be.Stateless.BizTalk.Pipeline.Components, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14");
      if (comp0.GetType().IsInstanceOfType(typeof(Microsoft.BizTalk.Component.Interop.IPersistPropertyBag)))
      {
        ((Microsoft.BizTalk.Component.Interop.IPersistPropertyBag)(comp0)).Load(new Microsoft.BizTalk.PipelineOM.PropertyBag(new System.Collections.ArrayList(new Microsoft.BizTalk.PipelineOM.PropertyContents[] {
          new Microsoft.BizTalk.PipelineOM.PropertyContents("Enabled", true),
          new Microsoft.BizTalk.PipelineOM.PropertyContents("EnableFailedMessageRouting", true),
          new Microsoft.BizTalk.PipelineOM.PropertyContents("SuppressRoutingFailureReport", true)})), 0);
      }
      this.AddComponent(stage, comp0);
      Microsoft.BizTalk.Component.Interop.IBaseComponent comp1 = Microsoft.BizTalk.PipelineOM.PipelineManager.CreateComponent("Be.Stateless.BizTalk.Component.MicroPipelineComponent, Be.Stateless.BizTalk.Pipeline.Components, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14");
      if (comp1.GetType().IsInstanceOfType(typeof(Microsoft.BizTalk.Component.Interop.IPersistPropertyBag)))
      {
        ((Microsoft.BizTalk.Component.Interop.IPersistPropertyBag)(comp1)).Load(new Microsoft.BizTalk.PipelineOM.PropertyBag(new System.Collections.ArrayList(new Microsoft.BizTalk.PipelineOM.PropertyContents[] {
          new Microsoft.BizTalk.PipelineOM.PropertyContents("Enabled", true),
          new Microsoft.BizTalk.PipelineOM.PropertyContents("Components", "")})), 0);
      }
      this.AddComponent(stage, comp1);
      stage = this.AddStage(Microsoft.BizTalk.PipelineOM.Stage.DisassemblingParser, Microsoft.BizTalk.PipelineOM.ExecutionMode.firstRecognized);
      Microsoft.BizTalk.Component.Interop.IBaseComponent comp2 = Microsoft.BizTalk.PipelineOM.PipelineManager.CreateComponent("Microsoft.BizTalk.Component.XmlDasmComp, Microsoft.BizTalk.Pipeline.Components, Version=3.0.1.0, Culture=neutral, PublicKeyToken=31bf3856ad364e35");
      if (comp2.GetType().IsInstanceOfType(typeof(Microsoft.BizTalk.Component.Interop.IPersistPropertyBag)))
      {
        ((Microsoft.BizTalk.Component.Interop.IPersistPropertyBag)(comp2)).Load(new Microsoft.BizTalk.PipelineOM.PropertyBag(new System.Collections.ArrayList(new Microsoft.BizTalk.PipelineOM.PropertyContents[] {
          new Microsoft.BizTalk.PipelineOM.PropertyContents("EnvelopeSpecNames", ""),
          new Microsoft.BizTalk.PipelineOM.PropertyContents("EnvelopeSpecTargetNamespaces", ""),
          new Microsoft.BizTalk.PipelineOM.PropertyContents("DocumentSpecNames", ""),
          new Microsoft.BizTalk.PipelineOM.PropertyContents("DocumentSpecTargetNamespaces", ""),
          new Microsoft.BizTalk.PipelineOM.PropertyContents("AllowUnrecognizedMessage", false),
          new Microsoft.BizTalk.PipelineOM.PropertyContents("ValidateDocument", false),
          new Microsoft.BizTalk.PipelineOM.PropertyContents("RecoverableInterchangeProcessing", false),
          new Microsoft.BizTalk.PipelineOM.PropertyContents("HiddenProperties", "EnvelopeSpecTargetNamespaces,DocumentSpecTargetNamespaces"),
          new Microsoft.BizTalk.PipelineOM.PropertyContents("DtdProcessing", "")})), 0);
      }
      this.AddComponent(stage, comp2);
      stage = this.AddStage(Microsoft.BizTalk.PipelineOM.Stage.Validator, Microsoft.BizTalk.PipelineOM.ExecutionMode.all);
      Microsoft.BizTalk.Component.Interop.IBaseComponent comp3 = Microsoft.BizTalk.PipelineOM.PipelineManager.CreateComponent("Be.Stateless.BizTalk.Component.MicroPipelineComponent, Be.Stateless.BizTalk.Pipeline.Components, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14");
      if (comp3.GetType().IsInstanceOfType(typeof(Microsoft.BizTalk.Component.Interop.IPersistPropertyBag)))
      {
        ((Microsoft.BizTalk.Component.Interop.IPersistPropertyBag)(comp3)).Load(new Microsoft.BizTalk.PipelineOM.PropertyBag(new System.Collections.ArrayList(new Microsoft.BizTalk.PipelineOM.PropertyContents[] {
          new Microsoft.BizTalk.PipelineOM.PropertyContents("Enabled", true),
          new Microsoft.BizTalk.PipelineOM.PropertyContents("Components", "")})), 0);
      }
      this.AddComponent(stage, comp3);
    }

    public override string XmlContent
    {
      get
      {
        return _strPipeline;
      }
    }

    private const string _strPipeline = @"<?xml version='1.0' encoding='utf-16'?>
<Document xmlns:xsi='http://www.w3.org/2001/XMLSchema-instance' xmlns:xsd='http://www.w3.org/2001/XMLSchema' MajorVersion='1' MinorVersion='0'>
  <Description>XML receive micro-pipeline.</Description>
  <CategoryId>f66b9f5e-43ff-4f5f-ba46-885348ae1b4e</CategoryId>
  <FriendlyName>Receive</FriendlyName>
  <Stages>
    <Stage>
      <PolicyFileStage _locAttrData='Name' _locID='1' Name='Decode' minOccurs='0' maxOccurs='-1' execMethod='All' stageId='9d0e4103-4cce-4536-83fa-4a5040674ad6' />
      <Components>
        <Component>
          <Name>Be.Stateless.BizTalk.Component.FailedMessageRoutingEnablerComponent, Be.Stateless.BizTalk.Pipeline.Components, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14</Name>
          <ComponentName>FailedMessageRoutingEnablerComponent</ComponentName>
          <Description>Enables routing of failed messages and prevents routing failure reports from being generated.</Description>
          <Version>2.0</Version>
          <Properties>
            <Property Name='Enabled'>
              <Value xsi:type='xsd:boolean'>true</Value>
            </Property>
            <Property Name='EnableFailedMessageRouting'>
              <Value xsi:type='xsd:boolean'>true</Value>
            </Property>
            <Property Name='SuppressRoutingFailureReport'>
              <Value xsi:type='xsd:boolean'>true</Value>
            </Property>
          </Properties>
          <CachedDisplayName>FailedMessageRoutingEnablerComponent</CachedDisplayName>
          <CachedIsManaged>true</CachedIsManaged>
        </Component>
        <Component>
          <Name>Be.Stateless.BizTalk.Component.MicroPipelineComponent, Be.Stateless.BizTalk.Pipeline.Components, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14</Name>
          <ComponentName>MicroPipelineComponent</ComponentName>
          <Description>Runs a sequence of micro components as if they were regular pipeline components.</Description>
          <Version>2.0</Version>
          <Properties>
            <Property Name='Enabled'>
              <Value xsi:type='xsd:boolean'>true</Value>
            </Property>
            <Property Name='Components'>
              <Value xsi:type='xsd:string' />
            </Property>
          </Properties>
          <CachedDisplayName>MicroPipelineComponent</CachedDisplayName>
          <CachedIsManaged>true</CachedIsManaged>
        </Component>
      </Components>
    </Stage>
    <Stage>
      <PolicyFileStage _locAttrData='Name' _locID='2' Name='Disassemble' minOccurs='0' maxOccurs='-1' execMethod='FirstMatch' stageId='9d0e4105-4cce-4536-83fa-4a5040674ad6' />
      <Components>
        <Component>
          <Name>Microsoft.BizTalk.Component.XmlDasmComp, Microsoft.BizTalk.Pipeline.Components, Version=3.0.1.0, Culture=neutral, PublicKeyToken=31bf3856ad364e35</Name>
          <ComponentName>XML disassembler</ComponentName>
          <Description>Streaming XML disassembler</Description>
          <Version>1.0</Version>
          <Properties>
            <Property Name='EnvelopeSpecNames'>
              <Value xsi:type='xsd:string' />
            </Property>
            <Property Name='EnvelopeSpecTargetNamespaces'>
              <Value xsi:type='xsd:string' />
            </Property>
            <Property Name='DocumentSpecNames'>
              <Value xsi:type='xsd:string' />
            </Property>
            <Property Name='DocumentSpecTargetNamespaces'>
              <Value xsi:type='xsd:string' />
            </Property>
            <Property Name='AllowUnrecognizedMessage'>
              <Value xsi:type='xsd:boolean'>false</Value>
            </Property>
            <Property Name='ValidateDocument'>
              <Value xsi:type='xsd:boolean'>false</Value>
            </Property>
            <Property Name='RecoverableInterchangeProcessing'>
              <Value xsi:type='xsd:boolean'>false</Value>
            </Property>
            <Property Name='HiddenProperties'>
              <Value xsi:type='xsd:string'>EnvelopeSpecTargetNamespaces,DocumentSpecTargetNamespaces</Value>
            </Property>
            <Property Name='DtdProcessing'>
              <Value xsi:type='xsd:string' />
            </Property>
          </Properties>
          <CachedDisplayName>XML disassembler</CachedDisplayName>
          <CachedIsManaged>true</CachedIsManaged>
        </Component>
      </Components>
    </Stage>
    <Stage>
      <PolicyFileStage _locAttrData='Name' _locID='3' Name='Validate' minOccurs='0' maxOccurs='-1' execMethod='All' stageId='9d0e410d-4cce-4536-83fa-4a5040674ad6' />
      <Components>
        <Component>
          <Name>Be.Stateless.BizTalk.Component.MicroPipelineComponent, Be.Stateless.BizTalk.Pipeline.Components, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14</Name>
          <ComponentName>MicroPipelineComponent</ComponentName>
          <Description>Runs a sequence of micro components as if they were regular pipeline components.</Description>
          <Version>2.0</Version>
          <Properties>
            <Property Name='Enabled'>
              <Value xsi:type='xsd:boolean'>true</Value>
            </Property>
            <Property Name='Components'>
              <Value xsi:type='xsd:string' />
            </Property>
          </Properties>
          <CachedDisplayName>MicroPipelineComponent</CachedDisplayName>
          <CachedIsManaged>true</CachedIsManaged>
        </Component>
      </Components>
    </Stage>
    <Stage>
      <PolicyFileStage _locAttrData='Name' _locID='4' Name='ResolveParty' minOccurs='0' maxOccurs='-1' execMethod='All' stageId='9d0e410e-4cce-4536-83fa-4a5040674ad6' />
      <Components />
    </Stage>
  </Stages>
</Document>";

    public override System.Guid VersionDependentGuid
    {
      get
      {
        return new System.Guid(_versionDependentGuid);
      }
    }

    private const string _versionDependentGuid = "2cdb242d-d0ba-4e55-995a-47632bddd5fc";
  }
}
```

<!-- badges -->

[doc.main.badge]: https://img.shields.io/static/v1?label=BizTalk.Factory%20SDK&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.main]: https://www.stateless.be/ "BizTalk.Factory SDK User's Guide"
[doc.this.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Pipelines&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.this]: https://www.stateless.be/BizTalk/Pipelines "Be.Stateless.BizTalk.Pipelines User's Guide"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.BizTalk.Pipelines&logo=github
[github]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipelines "Be.Stateless.BizTalk.Pipelines GitHub Repository"
[nuget.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Pipelines.svg?label=Be.Stateless.BizTalk.Pipelines&style=flat&logo=nuget
[nuget]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Pipelines "Be.Stateless.BizTalk.Pipelines NuGet Package"
[nuget.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/Be.Stateless.BizTalk.Pipelines?logo=nuget
[nuget.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=Be.Stateless.BizTalk.Pipelines&protocolType=NuGet "Be.Stateless.BizTalk.Pipelines Preview NuGet Package"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Pipelines%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=57&branchName=master "Be.Stateless.BizTalk.Pipelines Continuous Integration Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Pipelines%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=58&branchName=master "Be.Stateless.BizTalk.Pipelines Manual Release Build Pipeline"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.Pipelines?label=Release&logo=github
[release]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipelines/releases/latest "Be.Stateless.BizTalk.Pipelines Release"

<!-- links -->

[ff-receive]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipelines/blob/master/src/Be.Stateless.BizTalk.Pipeline.Definitions/MicroPipelines/FFReceive.cs
[ff-transmit]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipelines/blob/master/src/Be.Stateless.BizTalk.Pipeline.Definitions/MicroPipelines/FFTransmit.cs
[pass-thru-receive]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipelines/blob/master/src/Be.Stateless.BizTalk.Pipeline.Definitions/MicroPipelines/PassThruReceive.cs
[pass-thru-transmit]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipelines/blob/master/src/Be.Stateless.BizTalk.Pipeline.Definitions/MicroPipelines/PassThruTransmit.cs
[xml-receive]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipelines/blob/master/src/Be.Stateless.BizTalk.Pipeline.Definitions/MicroPipelines/XmlReceive.cs
[xml-transmit]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipelines/blob/master/src/Be.Stateless.BizTalk.Pipeline.Definitions/MicroPipelines/XmlTransmit.cs

<!-- images -->

[xml-receive.btp]: ./../../assets/images/XmlReceive.btp.png "XmlReceive Micro Pipeline"

<!--
cSpell:ignore typeof XmlDasmComp
-->
