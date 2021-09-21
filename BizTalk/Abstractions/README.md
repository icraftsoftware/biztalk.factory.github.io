# Be.Stateless.BizTalk.Abstractions Component

[![GitHub](https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.BizTalk.Abstractions&logo=github)][GitHub]

[![Build Status](https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Abstractions%20Manual%20Release?branchName=master)][Pipeline]

[![NuGet Version](https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Abstractions.svg?label=Be.Stateless.BizTalk.Abstractions&style=flat?style=plastic&logo=nuget)][NuGet Package]


## Overview

Be.Stateless.BizTalk.Abstractions is part of the [BizTalk.Factory Runtime Package](./../Factory/Runtime/README.md). This component provides caching and BizTalk Server's message context abstractions.

## Caching Abstractions

Caching abstractions provide both absolute and sliding expiration caches that are used pervasively in BizTalk.Factory to either cache for instance extracted schema metadata, compiled XSLTs, compiled regular expressions, and so on...

Further information can be found in the XML comments embedded in the source code and accompanying the [NuGet Package].

## Message Context Abstractions

There is some amount of idiosyncrasies coming with Microsoft BizTalk Server®, and reading, promoting, and writing context properties certainly come with its share of oddities.

First, accessing the context property must be done in two very distinct ways depending on whether the property needs to be accessed from an `IBaseMessage` or an `XLANGMessage` message object instance. The `IBaseMessage` API is even more awkward as one must most often instantiate some sort of context property descriptor object in order to get a QName that will allow one to ultimately get both the context property's local and namespace names to pass to the API method.

Next, the value returned is always of type object and it must always be casted to the exact concrete type of the property.

Finally, how to delete a property value from the message context as none of the `IBaseMessage` and `XLANGMessage` API expose a delete method. Does one have to assign to the property a null value or an empty string? Does this work the same way with both `IBaseMessage` and `XLANGMessage` APIs?

`IBaseMessage` Sample

`XLANGMessage` Sample

Would it not be better if there was a unique, regular, and type-safe way of accessing message context properties? Come `Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T, TR>` and `Be.Stateless.BizTalk.Message.Extensions.BaseMessage` classes to the rescue! With the help of these two classes, and provided the property to access has been defined in a property schema as a Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase-derived property, one now can simply write the following code.

Granted, this new API comes with a price: one has to define the context properties in one property schema, even though the original `IBaseMessage` API would not require it. All one needed to access a context property from an `IBaseMessage` was a couple of namespace and local name strings. This new requirement however comes with a huge benefit that far outweighs its drawback. Magic strings never have to be used any more, and namespace can never get out of sync between the `IBaseMessage` and `XLANGMessage` APIs.



## BizTalk Factory Context Property Schemas

BizTalk Factory comes with the following context property schemas, all packaged into the Be.Stateless.BizTalk.Schemas assembly:
•	Be.Stateless.BizTalk.Schemas.BizTalkFactory.Properties, whose XML target namespace is urn:schemas.stateless.be:biztalk:properties:system:2012:04,
•	Be.Stateless.BizTalk.Schemas.Tracking.Properties, whose XML target namespace is urn:schemas.stateless.be:biztalk:properties:tracking:2012:04,
•	BTS.UnexposedSystemProperties, whose XML target namespace is http://schemas.microsoft.com/BizTalk/2003/system-properties,
•	EDI.UnexposedEdiProperties, whose XML target namespace is http://schemas.microsoft.com/Edi/PropertySchema,



<!-- links -->
[GitHub]:https://github.com/icraftsoftware/Be.Stateless.BizTalk.Abstractions "Be.Stateless.BizTalk.Abstractions Git Repository"
[Pipeline]:https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=40&branchName=master "Azure DevOps Build Pipeline"
[NuGet Package]:https://www.nuget.org/packages/Be.Stateless.BizTalk.Abstractions/ "Be.Stateless.BizTalk.Abstractions NuGet Package"

<!--
cSpell:ignore XLANG biztalk
-->
