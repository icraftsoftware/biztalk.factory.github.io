# Be.Stateless.BizTalk.Pipeline.MicroComponents

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

`Be.Stateless.BizTalk.Pipeline.MicroComponents` is part of the [BizTalk.Factory Runtime](./../../Factory/Runtime/README.md) Package. This component provides various general purpose micro components meant to be run by the `BizTalk.Factory`'s [MicroPipelineComponent][micro-pipeline-component], see [Be.Stateless.BizTalk.Pipeline.Components](./../Components/README.md), [Be.Stateless.BizTalk.Pipelines](./../../Pipelines/README.md), [Be.Stateless.BizTalk.Dsl.Pipeline](./../../Dsl/Pipeline/README.md), and [Be.Stateless.BizTalk.Dsl.Binding](./../../Dsl/Binding/README.md) for more information about micro pipelines.

> **Remark** Being part of the `BizTalk.Factory Runtime`, this component's deployment only requires its assembly to be GAC-deployed; it consequently has no `BizTalkMgmtDb` footprint at all as it is not deployed as a Microsoft BizTalk Server® resource.

## Micro Components

`Be.Stateless.BizTalk.Pipeline.MicroComponents` comes with the following micro components:

- [Be.Stateless.BizTalk.MicroComponent.ContextBuilder][context-builder] which is a micro component that delegates the building of message context to a [IContextBuilder][i-context-builder] component plugin, either statically configured or discovered at runtime thanks to the [BizTalkFactoryProperties.ContextBuilderTypeName][biztalk-factory-properties.context-builder-type-name] context property, whose execution can be deferred until the message body's stream passing through is exhausted, see [PluginExecutionTime][plugin-execution-time];

- [Be.Stateless.BizTalk.MicroComponent.ContextPropertyExtractor][context-property-extractor] which allows to manipulate the message context by either clearing, demoting, writing or promoting property values. These values can either be constant or extracted out of an `XML` message by defining `XPath` expressions. These `XPath` extractors can be [statically configured][context-property-extractor.configuration-example] at the pipeline or be embedded as annotations &mdash;see their [grammar][context-property-extractor.annotation-grammar] and an [example][context-property-extractor.annotation-example]&mdash; in the `XML` schema of the message currently running through the micro component;

  > **Remark** At first sight, it might seem that this `ContextPropertyExtractor` micro component is a complete overlap of what Microsoft BizTalk Server® offers out of the box, see [Promoting Properties][promoting-properties] and [Property Schemas][property-schemas]. This `ContextPropertyExtractor` micro component however comes with real added value:
  >
  > 1. First of all, context properties can be written into context and not just promoted;
  >
  > 2. Then, the allowed `XPath` expressions are somewhat less restrictive than the traditional canonical `XPath` expressions supported by Microsoft BizTalk Server®, but limitations are however still present and relatively strong;
  >
  > 3. Finally, it circumvents an odd restriction requiring that the property schema associated with a message schema be in the same Microsoft BizTalk Server® project, &mdash;see note's first bullet at [Create property schema overview][create-property-schema-overview]. On rare occasions, this restriction prevents a Microsoft BizTalk Server® solution from compiling and leaves the developers to their own devices as Microsoft won't offer support for this scenario as stated clearly in the aforementioned note.

- [Be.Stateless.BizTalk.MicroComponent.DirectoryCreator][directory-creator] which allows to create folders before the `FILE` adapter drops a message as a file on disk. It can even impersonate any Windows identity thanks to the credentials provided by the `FILE` adapter configuration;

- [Be.Stateless.BizTalk.MicroComponent.FailedMessageRoutingEnabler][failed-message-routing-enabler] which enables routing of failed messages and prevents routing failure reports from being generated. The [Be.Stateless.BizTalk.Component.FailedMessageRoutingEnablerComponent][failed-message-routing-enabler-component] actually delegates to this micro component, see [Be.Stateless.BizTalk.Pipeline.Components](./../Components/README.md);

- [Be.Stateless.BizTalk.MicroComponent.MessageBodyStreamFactory][message-body-stream-factory] which replaces the stream of the current message's [BodyPart][i-base-message.body-part] by a new one whose creation is delegated to either a contextual, see [BizTalkFactoryProperties.MessageBodyStreamFactoryTypeName][biztalk-factory-properties.message-body-stream-factory-type-name] context property, or statically configured [IMessageBodyStreamFactory][i-message-body-stream-factory] plugin;

- [Be.Stateless.BizTalk.MicroComponent.MessageConsumer][message-consumer] which drains and consumes the pipeline's message;

- [Be.Stateless.BizTalk.MicroComponent.MessageTypeExtractor][message-type-extractor] which probes the current message for its type and write it in the [BizTalkFactoryProperties.MessageType][biztalk-factory-properties.message-type] context property.

- [Be.Stateless.BizTalk.MicroComponent.MultipartFormDataContentEncoder][multipart-form-data-content-encoder] which wraps the original message stream in a [MultipartFormDataContentStream][multipart-form-data-content-stream];

- [Be.Stateless.BizTalk.MicroComponent.SBMessagingContextPropagator][sb-messaging-context-propagator] which propagates outwards message type and correlation id over to Azure ServiceBus queued messages, and which propagates inwards correlation id from Azure ServiceBus queued messages;

- [Be.Stateless.BizTalk.MicroComponent.TransportRetriesDisabler][transport-retries-disabler] which prevents Microsoft BizTalk Server's SendPort Transport from performing any retries to send the message in case of failures;

- [Be.Stateless.BizTalk.MicroComponent.XmlEnvelopeDecoder][xml-envelope-decoder] which wraps the original message stream in a [XmlEnvelopeDecodingStream][xml-envelope-decoding-stream] to prevent the disassembler from throwing when some `XML` elements along the body XPath for envelope schemas are either missing or empty or self-closed, see [BizTalk envelope schema self-closing node](https://stackoverflow.com/q/22766952/1789441);

- [Be.Stateless.BizTalk.MicroComponent.XmlTranslator][xml-translator] which, on the fly, moves elements, and optionally attributes, from one `XML` namespace to another in the `XML` stream constituting the body of the message. The namespace translation to be made can either be statically configured or be discovered at runtime thanks to the [BizTalkFactoryProperties.XmlTranslations][biztalk-factory-properties.xml-translations] context property;

- [Be.Stateless.BizTalk.MicroComponent.XsltRunner][xslt-runner] which applies an `XSL` Transformation on `XML` messages along their way in the pipeline. The map can either be statically configured or discovered at runtime thanks to the [BizTalkFactoryProperties.MapTypeName][biztalk-factory-properties.map-type-name] context property;

- [Be.Stateless.BizTalk.MicroComponent.ZipDecoder][zip-decoder] which wraps the message's original stream in a [ZipInputStream][zip-input-stream] that decompresses the first entry of a Zip Archive;

- [Be.Stateless.BizTalk.MicroComponent.ZipEncoder][zip-encoder] which wraps the message's original stream in a [ZipOutputStream][zip-output-stream] that compresses it into a Zip Archive.

## Builder Plugins

`Be.Stateless.BizTalk.Pipeline.MicroComponents` comes with the following [IContextBuilder][i-context-builder] plugins:

- [FileOutboundTransportLocationBuilder][file-outbound-transport-location-builder] which computes the final destination path &mdash;folder path and file name&mdash; to be used by the `FILE` adapter on the basis of the destination folder configured at the adapter level &mdash;i.e. the configured destination folder without the file name&mdash; combined with the folder path and file name found in the context property [BizTalkFactoryProperties.OutboundTransportLocation][biztalk-factory-properties.outbound-transport-location];

- [SftpOutboundTransportLocationBuilder][sftp-outbound-transport-location-builder] which computes the final destination URI &mdash; server address, folder path, and file name&mdash; to be used by the `SFTP` adapter on the basis of the server address and folder path configured at the adapter level &mdash;i.e. the configured folder path without the file name&mdash; combined with the folder path and file name found in the context property [BizTalkFactoryProperties.OutboundTransportLocation][biztalk-factory-properties.outbound-transport-location].

## Developing and Testing Custom Pipeline Micro Components

<!-- TODO the development and unit testing of custom micro components is much easier and simpler to perform than it is for traditional Microsoft BizTalk Server® pipeline components. -->

1. Be.Stateless.BizTalk.Pipeline.MicroComponents.Unit
2. Be.Stateless.BizTalk.Pipeline.MicroComponents.NUnit
3. Be.Stateless.BizTalk.Pipeline.MicroComponents.XUnit

## Developer Help

Detailed developer help has been provided as `XML` comments directly embedded in source code. Though developers usually browse through this documentation while developing thanks to, for instance, JetBrains [ReSharper][resharper] quick help &mdash;<kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>F1</kbd>, an online version of this inlined help has also been provided here for greater reachability:

[![][help.badge]][help]

[![][help.unit.badge]][help.unit]

[![][help.nunit.badge]][help.nunit]

[![][help.xunit.badge]][help.xunit]

<!-- links -->

[help]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/Pipeline/MicroComponents/README.md "Be.Stateless.BizTalk.Pipeline.MicroComponents Developer Help"
[help.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Pipeline.MicroComponents&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help.unit]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/Pipeline/MicroComponents/Unit/README.md "Be.Stateless.BizTalk.Pipeline.MicroComponents.Unit Developer Help"
[help.unit.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Pipeline.MicroComponents.Unit&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help.nunit]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/Pipeline/MicroComponents/NUnit/README.md "Be.Stateless.BizTalk.Pipeline.MicroComponents.NUnit Developer Help"
[help.nunit.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Pipeline.MicroComponents.NUnit&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help.xunit]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/Pipeline/MicroComponents/XUnit/README.md "Be.Stateless.BizTalk.Pipeline.MicroComponents.XUnit Developer Help"
[help.xunit.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Pipeline.MicroComponents.XUnit&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[github]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents "Be.Stateless.BizTalk.Pipeline.MicroComponents GitHub Repository"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.BizTalk.Pipeline.MicroComponents&logo=github
[nuget]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Pipeline.MicroComponents "Be.Stateless.BizTalk.Pipeline.MicroComponents NuGet Package"
[nuget.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Pipeline.MicroComponents.svg?label=Be.Stateless.BizTalk.Pipeline.MicroComponents&style=flat&logo=nuget
[nuget.unit]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Pipeline.MicroComponents.Unit "Be.Stateless.BizTalk.Pipeline.MicroComponents.Unit NuGet Package"
[nuget.unit.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Pipeline.MicroComponents.Unit.svg?label=Be.Stateless.BizTalk.Pipeline.MicroComponents.Unit&style=flat&logo=nuget
[nuget.nunit]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Pipeline.MicroComponents.NUnit "Be.Stateless.BizTalk.Pipeline.MicroComponents.NUnit NuGet Package"
[nuget.nunit.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Pipeline.MicroComponents.NUnit.svg?label=Be.Stateless.BizTalk.Pipeline.MicroComponents.NUnit&style=flat&logo=nuget
[nuget.xunit]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Pipeline.MicroComponents.XUnit "Be.Stateless.BizTalk.Pipeline.MicroComponents.XUnit NuGet Package"
[nuget.xunit.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Pipeline.MicroComponents.XUnit.svg?label=Be.Stateless.BizTalk.Pipeline.MicroComponents.XUnit&style=flat&logo=nuget
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=66&branchName=master "Azure DevOps Continuous Integration Build Pipeline"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Pipeline.MicroComponents%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=67&branchName=master "Azure DevOps Release Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Pipeline.MicroComponents%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[release]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/releases/latest "Be.Stateless.BizTalk.Pipeline.MicroComponents Release"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents?label=Release&logo=github

<!--  -->

[biztalk-factory-properties.context-builder-type-name]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/afb0e9806a8f2aa3324695603c3481e52ce493b0/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/BizTalkFactoryProperties.cs#L28
[biztalk-factory-properties.map-type-name]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/afb0e9806a8f2aa3324695603c3481e52ce493b0/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/BizTalkFactoryProperties.cs#L30
[biztalk-factory-properties.message-body-stream-factory-type-name]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/afb0e9806a8f2aa3324695603c3481e52ce493b0/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/BizTalkFactoryProperties.cs#L31
[biztalk-factory-properties.message-type]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/afb0e9806a8f2aa3324695603c3481e52ce493b0/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/BizTalkFactoryProperties.cs#L32
[biztalk-factory-properties.outbound-transport-location]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/afb0e9806a8f2aa3324695603c3481e52ce493b0/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/BizTalkFactoryProperties.cs#L33
[biztalk-factory-properties.xml-translations]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/afb0e9806a8f2aa3324695603c3481e52ce493b0/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/BizTalkFactoryProperties.cs#L34
[context-builder]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/ContextBuilder.cs
[context-property-extractor.annotation-example]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Batching.Application/blob/fe67490bb71c19113e4a9450013d08037f591a7f/src/Be.Stateless.BizTalk.Batching.Schemas/Schemas/Xml/Batch.xsd#L28
[context-property-extractor.annotation-grammar]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/4237869affc170596d97abef5ad0f95d1f0b3717/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/ContextPropertyExtractor.cs#L107
[context-property-extractor.configuration-example]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Batching.Application/blob/fe67490bb71c19113e4a9450013d08037f591a7f/src/Be.Stateless.BizTalk.Factory.Batching.Binding/ReceiveLocations/PartReceiveLocationStub.cs#L44
[context-property-extractor]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/ContextPropertyExtractor.cs
[create-property-schema-overview]: https://docs.microsoft.com/en-us/biztalk/core/property-schemas#create-property-schema-overview
[directory-creator]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/DirectoryCreator.cs
[failed-message-routing-enabler-component]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.Components/blob/master/src/Be.Stateless.BizTalk.Pipeline.Components/Component/FailedMessageRoutingEnablerComponent.cs
[failed-message-routing-enabler]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/FailedMessageRoutingEnabler.cs
[file-outbound-transport-location-builder]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/Builder/Send/FileOutboundTransportLocationBuilder.cs
[i-base-message.body-part]: https://docs.microsoft.com/en-us/dotnet/api/microsoft.biztalk.message.interop.ibasemessage.bodypart
[i-context-builder]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/IContextBuilder.cs
[i-message-body-stream-factory]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/IMessageBodyStreamFactory.cs
[message-body-stream-factory]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/MessageBodyStreamFactory.cs
[message-consumer]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/MessageConsumer.cs
[message-type-extractor]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/MessageTypeExtractor.cs
[micro-pipeline-component]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.Components/blob/master/src/Be.Stateless.BizTalk.Pipeline.Components/Component/MicroPipelineComponent.cs
[multipart-form-data-content-encoder]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/MultipartFormDataContentEncoder.cs
[multipart-form-data-content-stream]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Stream/blob/master/src/Be.Stateless.BizTalk.Stream/Stream/MultipartFormDataContentStream.cs
[plugin-execution-time]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/PluginExecutionTime.cs
[promoting-properties]: https://docs.microsoft.com/en-us/biztalk/core/promoting-properties
[property-schemas]: https://docs.microsoft.com/en-us/biztalk/core/property-schemas
[sb-messaging-context-propagator]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/SBMessagingContextPropagator.cs
[sftp-outbound-transport-location-builder]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/Builder/Send/SftpOutboundTransportLocationBuilder.cs
[transport-retries-disabler]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/TransportRetriesDisabler.cs
[xml-envelope-decoder]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/XmlEnvelopeDecoder.cs
[xml-envelope-decoding-stream]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Stream/blob/master/src/Be.Stateless.BizTalk.Stream/Stream/XmlEnvelopeDecodingStream.cs
[xml-translator]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/XmlTranslator.cs
[xslt-runner]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/XsltRunner.cs
[zip-decoder]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/ZipDecoder.cs
[zip-encoder]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.MicroComponents/blob/master/src/Be.Stateless.BizTalk.Pipeline.MicroComponents/MicroComponent/ZipEncoder.cs
[zip-input-stream]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Stream/blob/master/src/Be.Stateless.BizTalk.Stream/Stream/ZipInputStream.cs
[zip-output-stream]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Stream/blob/master/src/Be.Stateless.BizTalk.Stream/Stream/ZipOutputStream.cs

<!--
cSpell:ignore BizTalkMgmtDb
-->
