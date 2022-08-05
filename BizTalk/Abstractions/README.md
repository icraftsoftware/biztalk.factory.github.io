# Be.Stateless.BizTalk.Abstractions

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

`Be.Stateless.BizTalk.Abstractions` is part of the [BizTalk.Factory Runtime](./../Factory/Runtime/README.md) Package. This component provides various abstractions over Microsoft BizTalk Server®'s message contexts and context properties.

## Message Context Abstractions

There is some amount of idiosyncrasies coming with Microsoft BizTalk Server® and the API to manipulate &mdash;i.e. reading, promoting, or writing&mdash; message context properties certainly comes with its shares of oddities.

### Message Context API

First and foremost, accessing the context property must be done in two very distinct ways depending on whether the property needs to be accessed from an `IBaseMessage` or an `XLANGMessage`-based message instance. The `IBaseMessage` API is even more awkward as one must most often instantiate some sort of context property descriptor in order to get a QName that will ultimately allow one to get both the context property's local and namespace names to pass to the API method.

Then, the value returned be the reading API is always of type `object` and it must always be _explicitly_ casted to the exact concrete type of the property, which requires extra caution to handle `null` values when reading value type properties.

Finally, deleting a property value from the message context is generally awkward as none of the `IBaseMessage` and `XLANGMessage` API exposes a `Delete()` method. Does one have to assign a null value or an empty string to the property? Does this work the same way with both `IBaseMessage` and `XLANGMessage` APIs?

Take a look at the following couple of code samples that demonstrate how to read context properties with the native APIs.

Sample 1 - Accessing context properties using the built-in `IBaseMessage` API.

```csharp
public void ProcessMessage(IBaseMessage message)
{
    ...

    var messageTypeProperty = new BTS.MessageType();
    string messageType = (string) message.Context.Read(
        messageTypeProperty.Name.Name,
        messageTypeProperty.Name.Namespace);

    var enqueuedTimeProperty = new SBMessaging.EnqueuedTimeUtc();
    object value = message.Context.Read(
        enqueuedTimeProperty.Name.Name,
        enqueuedTimeProperty.Name.Namespace);
    DateTime enqueuedTime = value != null ? (DateTime) value : default;

    ...
}
```

Sample 2 - Accessing context properties using the built-in `XLANGMessage` API.

```csharp
public void ProcessMessage(XLANGMessage message)
{
    ...

    string messageType = (string) message.GetPropertyValue(
        typeof(BTS.MessageType));

    object value = (DateTime) message.GetPropertyValue(
        typeof(SBMessaging.EnqueuedTimeUtc));
    DateTime enqueuedTime = value != null ? (DateTime) value : default;

    ...
}
```

Now, contrast them with the following 2 code excerpts that demonstrate the use of a unique, regular, and type-safe API to manipulate message context properties. This new strongly-typed API is made available through extension methods provided by [BaseMessage][base-message-extensions] as wrappers around the built-in `IBaseMessage` and `XLANGMessage` APIs.

Sample 3 - Accessing context properties using `BizTalk.Factory`'s `IBaseMessage` extension methods.

```csharp
public void ProcessMessage(IBaseMessage message)
{
    ...

    string messageType = message.GetProperty(BtsProperties.MessageType);

    DateTime? enqueuedTime = message.GetProperty(SBMessagingProperties.EnqueuedTimeUtc);

    ...
}
```

Sample 4 - Accessing context properties using `BizTalk.Factory`'s `XLANGMessage` extension methods.

```csharp
public void ProcessMessage(XLANGMessage message)
{
    ...

    string messageType = message.GetProperty(BtsProperties.MessageType);

    DateTime? enqueuedTime = message.GetProperty(SBMessagingProperties.EnqueuedTimeUtc);

    ...
}
```

Notice that besides being shorter, they are more importantly identical, regardless of whether the message is an `IBaseMessage` or an `XLANGMessage` instance. They do not require any explicit casting. They leverage [Nullable&lt;T&gt;][nullable] for properties that are value types and would otherwise not support `null` values without explicit special case handling.

For the record, `BizTalk.Factory` moreover provides `IBaseMessageContext` extension methods that support the exact same API to either delete, promote, read or write context properties given an `IBaseMessageContext` object, see [BaseMessageContext][base-message-context-extensions].

### MessageContextProperty<T, TR> Abstraction

The previous extension-method-based API comes with 2 requirements:

1. Each context property that needs to be accessed must derive from [MessageContextPropertyBase][message-context-property-base]. This usually means that the property must be defined as a `MessageContextPropertyBase` in a `Property` schema, but as one will see, the property could be defined in plain `C#` if one does not require the property to take part into subscription filters (e.g. send port's filters);

2. A [MessageContextProperty<T, TR>][message-context-property] _accelerator_ needs to be instantiated for each context property that needs to be accessed via this API.

While the original `IBaseMessage` API only requires a pair of namespace and local name strings, this API requires types to be defined. But this is not really an issue as the `XLANGMessage` API requires types to be defined anyway. The benefits of defining such types therefore far outweigh their costs:

- There can be no longer be usage discrepancies between both `IBaseMessage` and `XLANGMessage` APIs as the API is now the same whether the message object being used derives from one type or the other;

- Local and namespace names' magic strings never have to be used anymore;

- Properties are always handled in a type-safe way, even the value type ones.

Because instantiating these context property's type-accelerators on demand is tedious and cumbersome, `BizTalk.Factory` readily provides most of them as static properties defined in a bunch of classes:

- [BizTalkFactoryProperties][biztalk-factory-properties.accelerators] provides the accelerators for the context properties that belong to `BizTalk.Factory` and cannot be used in publication/subscription filters.\
  Note that `BizTalk.Factory` also provides accelerators for its context properties that are meant to be used in publication/subscription filters, see [BizTalk.Schemas' Property Schemas](..\Schemas\README.md#property-schemas);

- [BtsProperties][bts-properties.accelerators] provides the accelerators for the Microsoft BizTalk Server®'s core system context properties, see [BTS](https://docs.microsoft.com/en-us/dotnet/api/bts) namespace;

- [EdiProperties][edi-properties.accelerators] and [OverridableEdiProperties][overridable-edi-properties.accelerators] provides the accelerators for the Microsoft BizTalk Server®'s `EDI` context properties, see [EDI](https://docs.microsoft.com/en-us/dotnet/api/edi) and [EdiOverride](https://docs.microsoft.com/en-us/dotnet/api/edioverride) namespaces;

- [ErrorReportProperties][error-report-properties.accelerators] provides the accelerators for the Microsoft BizTalk Server®'s context properties related to error reporting, see [ErrorReport](https://docs.microsoft.com/en-us/dotnet/api/errorreport) namespace;

- [FileProperties][file-properties.accelerators] provides the accelerators for the Microsoft BizTalk Server®'s context properties related to the `File` adapter, see [FILE](https://docs.microsoft.com/en-us/dotnet/api/file) namespace;

- [HttpProperties][http-properties.accelerators] provides the accelerators for the Microsoft BizTalk Server®'s context properties related to the `HTTP` adapter, see [HTTP](https://docs.microsoft.com/en-us/dotnet/api/http) namespace;

- [Pop3Properties][pop3-properties.accelerators] provides the accelerators for the Microsoft BizTalk Server®'s context properties related to the `POP3` adapter, see [POP3](https://docs.microsoft.com/en-us/dotnet/api/pop3) namespace;

- [SBMessagingProperties][sb-messaging-properties.accelerators] provides the accelerators for the Microsoft BizTalk Server®'s context properties related to the `SB-Messaging` adapter, see [SBMessaging](https://docs.microsoft.com/en-us/dotnet/api/sbmessaging) namespace.

> **Remark** Take notice of another Microsoft BizTalk Server® oddity: the `SB-Messaging` adapter does not make use of the `CustomBrokeredMessagePropertyNamespace` context property in its own `XML` namespace, but uses instead the `CustomBrokeredPropertyNamespace` context property in the [WCF](https://docs.microsoft.com/en-us/dotnet/api/wcf) `XML` namespace, see [WcfProperties][wcf-properties.accelerators];

- [SapProperties][sap-properties.accelerators] provides the accelerators for the Microsoft BizTalk Server®'s context properties related to the `SAP` adapter, see [Message Context Properties for Receiving IDOCs](https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-sap/message-context-properties-for-receiving-idocs);

- [SftpProperties][sftp-properties.accelerators] provides the accelerators for the Microsoft BizTalk Server®'s context properties related to the `SFTP` adapter, see [SFTP](https://docs.microsoft.com/en-us/dotnet/api/sftp) namespace;

- [WcfProperties][wcf-properties.accelerators] provides the accelerators for the Microsoft BizTalk Server®'s context properties related to the `WCF` adapters, see [WCF](https://docs.microsoft.com/en-us/dotnet/api/wcf) namespace.

## Context Properties

For each context property that needs to be accessed via the previously mentioned API, a type deriving from `MessageContextPropertyBase` must be defined so that its `MessageContextProperty<T, TR>` accelerator counterpart can be defined in turn.

However, not all of the standard or out-of-box context properties are backed by property schemas. They therefore do not have a corresponding `MessageContextPropertyBase`-derived type definition. To make these properties nonetheless usable through the `BizTalk.Factory` API, `Be.Stateless.BizTalk.Abstractions` fills the gap and provides plain `C#` type definitions &mdash;or pseudo property schemas&mdash; for the most meaningful ones.

> **Remark** These context properties only need a plain `C#` type definition and should not be backed by property schemas as they are not intended to be used in publication/subscription filters.

- [BizTalkFactory.Properties][biztalk-factory.properties] declares types for `BizTalk.Factory`'s own context properties that cannot be used in subscription filters;

- [Edi.Properties][edi.properties] declares types for `EDI` context properties that do not have a corresponding `MessageContextPropertyBase`-derived type definition;

- [Sftp.Properties][sftp.properties] declares types for `SFTP` context properties that do not have a corresponding `MessageContextPropertyBase`-derived type definition;

- [System.Properties][system.properties] declares types for `BTS` core system context properties that do not have a corresponding `MessageContextPropertyBase`-derived type definition.

> **Remark** Because these context properties now have corresponding type definitions, they can finally be used in [XLANG/s](https://docs.microsoft.com/en-us/biztalk/core/xlang-s-language) expressions too, for instances:\
> `variable = message(EDI.BGM1_1)`\
> or\
> `message(Be.Stateless.BizTalk.Schemas.BizTalkFactory.DisableTransportRetries) = true`.\
> They still, nonetheless, cannot be used in a subscription filter or correlation set.

### Fluent API

`Be.Stateless.BizTalk.Abstractions` also provides a fluent API, thanks to extension methods defined by the various classes in the [Be.Stateless.BizTalk.ContextProperties.Extensions][context-properties-extensions] namespace, to speed up and chain the assignment of the context properties it defines or brings to the surface.

## Developer Help

Detailed developer help has been provided as `XML` comments directly embedded in source code. Though developers usually browse through this documentation while developing thanks to, for instance, JetBrains [ReSharper][resharper] quick help &mdash;<kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>F1</kbd>, an online version of this inlined help has also been provided here for greater reachability:

[![][help.badge]][help]

<!-- badges -->

[doc.main.badge]: https://img.shields.io/static/v1?label=BizTalk.Factory%20SDK&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.main]: https://www.stateless.be/ "BizTalk.Factory SDK User's Guide"
[doc.this.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Abstractions&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.this]: https://www.stateless.be/BizTalk/Abstractions "Be.Stateless.BizTalk.Abstractions User's Guide"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.BizTalk.Abstractions&logo=github
[github]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions "Be.Stateless.BizTalk.Abstractions GitHub Repository"
[help.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Abstractions&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/Abstractions/README.md "Be.Stateless.BizTalk.Abstractions Developer Help"
[nuget.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Abstractions.svg?label=Be.Stateless.BizTalk.Abstractions&style=flat&logo=nuget
[nuget]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Abstractions "Be.Stateless.BizTalk.Abstractions NuGet Package"
[nuget.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/Be.Stateless.BizTalk.Abstractions?logo=nuget
[nuget.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=Be.Stateless.BizTalk.Abstractions&protocolType=NuGet "Be.Stateless.BizTalk.Abstractions Preview NuGet Package"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Abstractions%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=39&branchName=master "Be.Stateless.BizTalk.Abstractions Continuous Integration Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Abstractions%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=40&branchName=master "Be.Stateless.BizTalk.Abstractions Manual Release Build Pipeline"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.Abstractions?label=Release&logo=github
[release]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/releases/latest "Be.Stateless.BizTalk.Abstractions GitHub Release"

<!-- links -->

[base-message-context-extensions]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/Message/Extensions/BaseMessageContext.cs "Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext"
[base-message-extensions]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/Message/Extensions/BaseMessage.cs "Be.Stateless.BizTalk.Message.Extensions.BaseMessage"
[biztalk-factory-properties.accelerators]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/BizTalkFactoryProperties.cs
[biztalk-factory.properties]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/Schemas/BizTalkFactory/Properties.cs
[bts-properties.accelerators]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/BtsProperties.cs
[context-properties-extensions]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/tree/master/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/Extensions
[edi-properties.accelerators]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/EdiProperties.cs
[edi.properties]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/Schemas/Edi/Properties.cs
[error-report-properties.accelerators]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/ErrorReportProperties.cs
[file-properties.accelerators]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/FileProperties.cs
[http-properties.accelerators]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/HttpProperties.cs
[message-context-property-base]: https://docs.microsoft.com/en-us/dotnet/api/microsoft.xlangs.basetypes.messagecontextpropertybase?view=bts-2020 "Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase"
[message-context-property]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/MessageContextProperty.cs "Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T, TR>"
[nullable]: https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/nullable-value-types
[overridable-edi-properties.accelerators]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/OverridableEdiProperties.cs
[pop3-properties.accelerators]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/Pop3Properties.cs
[resharper]: https://www.jetbrains.com/resharper/
[sap-properties.accelerators]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/SapProperties.cs
[sb-messaging-properties.accelerators]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/SBMessagingProperties.cs
[sftp-properties.accelerators]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/SftpProperties.cs
[sftp.properties]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/Schemas/Sftp/Properties.cs
[system.properties]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/Schemas/System/Properties.cs
[wcf-properties.accelerators]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/WcfProperties.cs

<!--
cSpell:ignore biztalk overridable typeof XLANG
-->
