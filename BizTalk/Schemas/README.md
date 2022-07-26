# Be.Stateless.BizTalk.Schemas

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

</div>
</div>

## Overview

`Be.Stateless.BizTalk.Schemas` is part of the [BizTalk.Factory Application](./../Factory/Application/README.md) Package. This component provides `BizTalk.Factory`'s document and property schemas for general purpose Microsoft BizTalk Server® development.

## XML Schemas

`Be.Stateless.BizTalk.Schemas` comes with 2 generic `XML` schemas:

- [Any.xsd][any.xsd], whose type's full name is `Be.Stateless.BizTalk.Schemas.Xml.Any`, which is as its name suggests an `XML` schema for any `XML` document instance;

- [Envelope.xsd][envelope.xsd], whose type's full name is `Be.Stateless.BizTalk.Schemas.Xml.Envelope`, which is a generic and reusable envelope schema.

## Property Schemas

`Be.Stateless.BizTalk.Schemas` comes with 1 property schema, [BizTalkFactoryProperties.xsd][subscribable.biztalk-factory-properties.xsd], whose type's full name is `Be.Stateless.BizTalk.Schemas.BizTalkFactory.Properties`, and which defines 3 properties that can be used in message routing scenarios, i.e. publication/subscription filters:

- `CorrelationId`, which denotes the identifier of the correlation;

- `EnvironmentTag`, which is to be used when one Microsoft BizTalk Server® application has to be connected to several distinct and non-overlapping sets of interacting parties &mdash;or environments&mdash; and cannot leak messages from one set of parties into another. In concrete terms, it is meant to be used in pub/sub scenarios &mdash;i.e. promoted into message context with a pending subscription filter&mdash; in order to keep messages strictly insulated within a particular set of such interacting parties;

- `ReceiverName`, which denotes the name of the intended receiver of the current message. This is a generic token not to be confused with a ReceivePort name;

- `SenderName`, which denotes the name of the initiating sender of the current message. This is a generic token not to be confused with a ReceivePort name;

## Context Properties

Following the `BizTalk.Factory` design principles, [Be.Stateless.BizTalk.ContextProperties.**Subscribable**.BizTalkFactoryProperties][subscribable.biztalk-factory-properties.accelerators] provides the accelerators for the context properties that belong to `BizTalk.Factory` and can be used in subscription filters. These are not to be confused with [Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties][biztalk-factory-properties.accelerators], which provides the accelerators for the context properties that cannot be used in subscription filters.

> See [Message Context API](./../Abstractions/README.md#message-context-api) and [MessageContextProperty<T, TR> Abstraction](./../Abstractions/README.md#messagecontextpropertyt-tr-abstraction) for background information about these accelerators.

### Fluent API

`Be.Stateless.BizTalk.Schemas` also provides a fluent API, thanks to extension methods defined by [Be.Stateless.BizTalk.ContextProperties.Extensions.BizTalkFactorySubscribablePropertiesExtensions][biztalk-factory-subscribable-properties-extensions], to speed up and chain the assignment or the promotion of the context properties it defines.

## Unit Testing Library

<!-- TODO resourceManager.Load<xxx>(sampleResource) -->

`Be.Stateless.BizTalk.Schemas.Unit` provides helper classes and methods to write unit tests that will help the developers to avoid awkward and frustrating situations. It comes with 2 seemingly innocuous extensions methods that retrieve all the message types or schema strong names that cannot be promoted because they exceed 256 characters, see [GetUnpromotableMessageTypes][get-unpromotable-message-types] and [GetUnpromotableSchemaStrongNames][get-unpromotable-schema-strong-names]. With the help of these methods, the developers can then guard against such problems by means of automated tests similar to the following:

```csharp
[Fact]
public void GetUnpromotableMessageTypes()
{
    schemaAssembly.GetUnpromotableMessageTypes().Should().BeEmpty();
}

[Fact]
public void GetUnpromotableSchemaStrongNames()
{
    schemaAssembly.GetUnpromotableSchemaStrongNames().Should().BeEmpty();
}
```

> **Remark** The predicate equivalents of these 2 methods are also available, see [IsPromotableMessageType][is-promotable-message-type] and [IsPromotableSchemaStrongName][is-promotable-schema-strong-name].

`Be.Stateless.BizTalk.Schemas.Unit` more importantly also provides a test base class, [Be.Stateless.BizTalk.Unit.Schema.SchemaFixture\<T>][schema-fixture], to validate that `XML` instance document are valid with respect to their `XML` schema. For instance:

```csharp
public class BatchFixture : SchemaFixture<Batch>
{
    [Theory]
    [InlineData("BatchContent.xml")]
    [InlineData("BatchContentWithEnvelopeSpecName.xml")]
    [InlineData("BatchContentWithEnvironmentTag.xml")]
    [InlineData("BatchContentWithEnvironmentTagAndPartition.xml")]
    [InlineData("BatchContentWithPartition.xml")]
    public void ValidateBatchContent(string resourceName)
    {
        Invoking(() => ValidateInstanceDocument(ResourceManager.Load(resourceName))).Should().NotThrow();
    }

    [Fact]
    public void PerformLaxValidation()
    {
        ValidateInstanceDocument(ResourceManager.Load("resource"), XmlSchemaContentProcessing.Lax);
    }

    ...

}
```

Writing these tests is particularly useful to ensure that, for instance, when the developers automate the tests of the `XSLT` maps, the input `XML` instance documents used to test the maps remain valid with respect to their `XML` schemas.

<!--
TODO
but map/transformFixture unit also provide a given input with validation
 -->

<!-- links -->

[github]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Schemas "Be.Stateless.BizTalk.Schemas GitHub Repository"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.BizTalk.Schemas&logo=github
[nuget]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Schemas "Be.Stateless.BizTalk.Schemas NuGet Package"
[nuget.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Schemas.svg?label=Be.Stateless.BizTalk.Schemas&style=flat?style=plastic&logo=nuget
[nuget.unit]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Schema.Unit "Be.Stateless.BizTalk.Schemas.Unit NuGet Package"
[nuget.unit.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Schema.Unit.svg?label=Be.Stateless.BizTalk.Schema.Unit&style=flat&logo=nuget
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=71&branchName=master "Azure DevOps Continuous Integration Build Pipeline"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Schemas%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=72&branchName=master "Azure DevOps Release Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Schemas%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[release]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Schemas/releases/latest "Be.Stateless.BizTalk.Schemas Release"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.Schemas?label=Release&logo=github
[any.xsd]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Schemas/blob/master/src/Be.Stateless.BizTalk.Schemas/Schemas/Xml/Any.xsd
[biztalk-factory-properties.accelerators]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions/blob/master/src/Be.Stateless.BizTalk.Abstractions/ContextProperties/BizTalkFactoryProperties.cs
[biztalk-factory-subscribable-properties-extensions]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Schemas/blob/master/src/Be.Stateless.BizTalk.Schemas/ContextProperties/Extensions/BizTalkFactorySubscribablePropertiesExtensions.cs
[subscribable.biztalk-factory-properties.xsd]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Schemas/blob/master/src/Be.Stateless.BizTalk.Schemas/Schemas/BizTalkFactoryProperties.xsd
[subscribable.biztalk-factory-properties.accelerators]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Schemas/blob/master/src/Be.Stateless.BizTalk.Schemas/ContextProperties/Subscribable/BizTalkFactoryProperties.cs
[envelope.xsd]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Schemas/blob/master/src/Be.Stateless.BizTalk.Schemas/Schemas/Xml/Envelope.xsd
[get-unpromotable-message-types]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Schemas/blob/b4914b7b2f4a3dd3692b24b97053e12b686cc994/src/Be.Stateless.BizTalk.Schema.Unit/Extensions/SchemaAssemblyExtensions.cs#L36
[get-unpromotable-schema-strong-names]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Schemas/blob/b4914b7b2f4a3dd3692b24b97053e12b686cc994/src/Be.Stateless.BizTalk.Schema.Unit/Extensions/SchemaAssemblyExtensions.cs#L43
[is-promotable-message-type]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Schemas/blob/b4914b7b2f4a3dd3692b24b97053e12b686cc994/src/Be.Stateless.BizTalk.Schema.Unit/Extensions/SchemaTypeExtensions.cs#L26
[is-promotable-schema-strong-name]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Schemas/blob/b4914b7b2f4a3dd3692b24b97053e12b686cc994/src/Be.Stateless.BizTalk.Schema.Unit/Extensions/SchemaTypeExtensions.cs#L31
[schema-fixture]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Schemas/blob/master/src/Be.Stateless.BizTalk.Schema.Unit/Unit/Schema/SchemaFixture.cs

<!--
cSpell:ignore messagecontextpropertyt-tr-abstraction unpromotable
-->
