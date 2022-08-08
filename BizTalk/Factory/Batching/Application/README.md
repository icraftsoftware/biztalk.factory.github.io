# BizTalk.Factory.Batching Application

[![][github.badge]][github]

##### Build Pipelines

[![][pipeline.mr.badge]][pipeline.mr]

[![][pipeline.ci.badge]][pipeline.ci]

##### Latest Release

[![][package.badge]][package]

[![][nuget.badge]][nuget]

[![][nuget.schemas.badge]][nuget.schemas]

[![][nuget.maps.badge]][nuget.maps]

[![][nuget.unit.badge]][nuget.unit]

[![][release.badge]][release]

##### Release Preview

<!-- TODO preview deployment packages -->

[![][nuget.preview.badge]][nuget.preview]

[![][nuget.schemas.preview.badge]][nuget.schemas.preview]

[![][nuget.maps.preview.badge]][nuget.maps.preview]

[![][nuget.unit.preview.badge]][nuget.unit.preview]

## Overview

`BizTalk.Factory.Batching` is an application add-on for Microsoft BizTalk Server® that provides rich and performant batching capabilities. `BizTalk.Factory.Batching` Application Package is part of the larger [BizTalk.Factory](./../../../../README.md) SDK and is made of the following components:

- [Be.Stateless.BizTalk.Factory.Batching.Schemas][nuget.schemas], which is a `NuGet` package providing schemas definitions and who is obviously meant to be referenced at development time;
- [Be.Stateless.BizTalk.Factory.Batching.Maps][nuget.maps], which is a `NuGet` package providing message transformation maps and who is obviously meant to be referenced at development time;
- [Be.Stateless.BizTalk.Factory.Batching][nuget], which is a `NuGet` package providing all other components &mdash;e.g. context builders, micro components, customized activity tracker...&mdash; necessary for this application and who is obviously meant to be referenced at development time;
- [Be.Stateless.BizTalk.Factory.Batching.Application.Deployment.zip][package], which is the whole application add-on itself and is meant to be deployed on Microsoft BizTalk Server®.

## Rationale

Microsoft BizTalk Server® comes with a strong debatching experience thanks to its disassembler pipeline components —that can as well be run within orchestrations;— debatching is therefore easy and performant. Deceivingly, the Microsoft BizTalk Server® _batching_ experience is very weak. There is no fully functional batching subsystem offered out of the box but only building blocks that are hard to put in place efficiently and correctly, i.e. without affecting the scalability and throughput of the platform. Indeed, most of the known and documented batching/aggregator patterns are based on orchestrations and exhibit either one or all of the following limitations:

- Batching orchestration instances are usually designed to wait for either a new part message to aggregate or a control message to trigger the release of the batch and all its parts accumulated so far. There is an inherent race condition with this design, which manifests itself when both a new part message and a release control message reach the orchestration at the same time. Most of the orchestration designs will fall short in this situation and lead to the following operational issue: "_The [batching orchestration] instance completed without consuming all of its messages. The instance and its unconsumed messages have been suspended._" Fixing the design of the batching orchestration to accommodate for this race condition can only be done, if at all possible, at the expense of an unjustified excessive increase in complexity.

- Batching orchestration instances see their performance gradually decrease as the number of accumulated parts increases. When releasing a batch that is made of 1000 parts or more, it is not unusual that the orchestration takes over 10 minutes to process, that is to say, to construct and send out the envelope message. As one can guess, there certainly is a linear correlation between the orchestration processing time and the number of aggregated parts. Even worse, the longer it takes to process the release of a batch, the more badly designed orchestrations will be exposed to the previously mentioned race condition issue.

- One cannot examine or edit the content of a batch under construction &mdash;i.e. the parts that have been accumulated so far&mdash; unless at the expense of a relatively complex development. The message parts, which constitute the state of the batching orchestration, are indeed serialized to the message box, which is an opaque repository. Consequently, any serialized orchestration state, and a fortiori its accumulated message parts, cannot be manually edited. One has therefore no other option than to create custom code to release the batch and process it through an alternate process that will allow its parts to be edited before being accumulated all over again.

`BizTalk Factory` departs from an orchestration-based batching solution and instead offers a Microsoft SQL Server® based batching subsystem that directly addresses all of the latter issues. The operational issues that arise consequently to the occurrences of the race condition with the orchestration-based design have gone. Though the race condition still subsists with the `BizTalk Factory`'s `Batching Application`, it has been addressed at the database level and no more can the release of a batch ends up being suspended. The batch release process, i.e. the construction of the message envelope, is performed by the database in nearly constant time, even for a very large number of accumulated parts. At any time, one can have a look at or edit the content of a batch or its parts through simple `T-SQL` statements.

## Batching Application Concepts

From the surface, the `BizTalk Factory`'s `Batching Application` is made up of a series of send ports and one receive location whose purpose is either to accumulate message parts out of the Microsoft BizTalk Server® message box, or queue the release of batches upon reception of control messages, or inject the content of batches just released into the Microsoft BizTalk Server® message box. Before looking into the technical details on how these concrete Microsoft BizTalk Server® artifacts interact and operate to deliver the `BizTalk Factory`'s `Batching Application`, there are a few distinguishing features that should be grasped.

### Envelope Schemas and Partitions

Without surprise, the `Batching Application` of `BizTalk Factory` is intrinsically related to an envelope schema —technically an `EnvelopeSpecName`— but it also intrinsically relies on the notion of partition. Conceptually, batch partitioning is some sort of constrain that ensures that, when releasing a batch and its parts, only the parts belonging to the same partition will be aggregated together within one envelope message. Technically, a batch must therefore be denoted by both an envelope schema and a partition.

Notice that even though envelope schemas must be registered to enable the `Batching Application` to start accumulating parts, partitions, which are just string labels, are totally dynamic and do not require any prior registration. Moreover, partitions are also optional and parts do not have to belong to any partition to be accumulated. Technically though, when a part being accumulated has no belonging partition, it will be associated to the default `0` (zero) partition.

### Batch Releases and Batch Release Policies

Batches can be released either upon the reception of a control message —that is an instance of the `Xml.Release` message schema/type— or according to some release policies that are periodically evaluated. These release policies, which can be configured at the batch level &mdash;whether partitioned or not,&mdash; are based on the following parameters:

- `Enabled`: For a given batch, designated by an `EnvelopeSpecName` and `Partition` couple, this parameter denotes whether the release policy for the batch is enabled or not. Disabling a release policy also prevents batches from being released via control messages.

- `Partition`: Denotes the specific partition of the related `EnvelopeSpecName` for which this release policy applies. If no partition is explicitly specified, it defaults to the `0` partition.

- `ReleaseOnIdleTimeOut`: For a given batch, designated by an `EnvelopeSpecName` and `Partition` couple, this parameter denotes the maximum amount of time that can elapse, since the last accumulated batch item or part, before the batch is automatically released.

- `ReleaseOnElapsedTimeOut`: For a given batch, designated by an `EnvelopeSpecName` and `Partition` couple, this parameter denotes the maximum amount of time that can elapse, since the very first accumulated batch item or part, before the batch is automatically released. It also ensures that a batch will eventually be released independently of the sliding nature of the `ReleaseOnIdleTimeOut` criterion.

- `ReleaseOnItemCount`: For a given batch, designated by an `EnvelopeSpecName` and `Partition` couple, this parameter denotes the minimum number of batch items or parts that can be accumulated before the batch is automatically released.

- `EnforceItemCountLimitOnRelease`: For a given batch, designated by an `EnvelopeSpecName` and `Partition` couple, this parameter denotes whether the `ReleaseOnItemCount` parameter is also used to enforce a maximum size limit on the number of batch items or parts that can be released together in a single envelope message. If the `EnforceItemCountLimitOnRelease` criterion is disabled, then all the batch items or parts that have been accumulated so far for a given batch will be released altogether.

Among these parameters, only the `Enabled` one is mandatory. Consequently if none of the optional parameters have been configured, batches will never be released automatically and only control messages would allow to release them.

Moreover, neither the reception of a control message nor the satisfaction of some release policy will trigger the **immediate** release of a batch; they will rather schedule the imminent release of batch. The actual release will indeed happen when Microsoft BizTalk Server® polls for the batches ready to be released, at which time, all the available batches will be released in a row, one after the other.

## Batching Application Design

The following diagram provides a general overview of how the `BizTalk Factory`'s `Batching Application` is materialized within Microsoft BizTalk Server®. At its perimeter, there are a couple of static one-way send ports and a single one-way receive location.

<a name="BatchingApplicationDesignOverview">![Batching Application Design Overview][application.design]</a>

- `BizTalk.Factory.Batching.SP1.Batch.Part.WCF-SQL.XML`, which is meant to aggregate parts for a given envelope. This send port actually subscribes to any message having a `Batch.EnvelopeSpecName` property promoted in context and will store its `XML` payload in database as a part of the corresponding batch, which is denoted by the `Batch.EnvelopeSpecName` and `Batch.EnvelopePartition` context properties, should the message have both, or denoted by the `Batch.EnvelopeSpecName` context property and the default `0` partition, should the message have no given partition in context.

  Notice that only the `Batch.EnvelopeSpecName` context property is part of the send port’s filter subscription, and consequently only it must be promoted in context; the `Batch.EnvelopePartition` context property, should it be present, simply has to be written in context.

- `BizTalk.Factory.Batching.SP1.Batch.Release.WCF-SQL.XML`, which is meant to schedule a batch for imminent release upon reception of a control message. This send port subscribes to any message being an instance of the `Xml.Release` schema/type.

- `BizTalk.Factory.Batching.RL1.Batch.Content.WCF-SQL.XML`, which is actually responsible of releasing a batch, that is to say its envelope and all its parts. This receive location regularly polls the database for the next available batch to release, whether releasable because a release policy has become satisfied at poll time or because a release control message has been received earlier. Recall that all the available batches will be released in a row, but one after the other to avoid saturating the receive location and the message box with a potentially large set of potentially big envelope messages arriving all at once.

  Notice that when an envelope message is published to the message box, its partition will be promoted, via the `Batch.EnvelopePartition` context property, on top of its message type, via the `BTS.MessageType` context property, as usual.

> **Remark** All the CLR property names and message type names that have been used in the preceding description about the BizTalk Server send ports and receive location were trimmed from their `Be.Stateless.BizTalk.Schemas` prefix for the sake of readability. In reality, the complete and correct CLR name for the `Batch.EnvelopeSpecName` property is `Be.Stateless.BizTalk.Schemas.Batch.EnvelopeSpecName`, and, for the `Xml.Release` message type is `Be.Stateless.BizTalk.Schemas.Xml.Batch.Release`.

> **Caution!** `Batch.EnvelopeSpecName` is not to be confused with `BTS.EnvelopeSpecName`. `BizTalk Factory` has deliberately chosen to use an equivalent property but in a different namespace to totally insulate its `Batching Application` from any batch-related feature built in Microsoft BizTalk Server®.

### Release Control Message

The release control message is used to schedule an imminent release of a given batch and has the following structure, where the `EnvelopeSpecName` is mandatory and the `Partition` is optional. Its CLR full name is `Be.Stateless.BizTalk.Schemas.Xml.Batch.Release`, while its `XML` message type is `urn:schemas.stateless.be:biztalk:batch:2012:12#ReleaseBatch`.

<a name="BatchReleaseControlMessageStructure">![Batch Release Control Message Structure][batch.release.message]</a>

Recall that a batch is unequivocally denoted by an envelope schema —technically an `EnvelopeSpecName—` and a `Partition`. As a consequence, failing to specify a partition in the release control message will only release the default `0` partition of a batch, and no other partition should there be more than one.

However, this message also accepts the `*` (any) wildcard instead of either the `EnvelopeSpecName` or the `Partition` elements, or both. One could therefore easily release all the partitions of a given envelope schema (the message would specify a given `EnvelopeSpecName` but a `*` `Partition`), or only a given partition irrespectively of the envelope schema (the message would specify a `*` `EnvelopeSpecName` and a given `Partition`), or all the batches having been accumulated so far, whatever the envelope schema and partition (the message would specify a `*` `EnvelopeSpecName` and `Partition`).

### Batch Content Message

As depicted at [Batching Application Design Overview](#BatchingApplicationDesignOverview "Batching Application Design Overview"), the `BizTalk.Factory.Batching.RL1.Batch.Content.WCF-SQL.XML` receive location relies on a `T-SQL` stored procedure, `usp_batch_ReleaseNextBatch`, to receive a message with the content of a given batch. Technically, this stored procedure is used to build the batch content message, whose structure is depicted below. Its CLR full name is `Be.Stateless.BizTalk.Schemas.Xml.Batch.Content`, while its `XML` message type is `urn:schemas.stateless.be:biztalk:batch:2012:12#BatchContent`. Only the `EnvelopeSpecName`, `Partition`, and `Parts` elements should be familiar; the `ProcessActivityId` and `MessagingStepActivityIds` elements will be described in the subsequent Batching Application Activity Monitoring section.

Notice that this batch content message is not the expected envelope message as it is clearly not an instance document of the envelope schema referenced by the `EnvelopeSpecName` element. This batch content message is indeed a private message &mdash;i.e. internal to the `BizTalk Factory`'s `Batching Application`&mdash; that has still to undergo some transformation to finally correspond to the expected envelope schema. This is the topic of the following section, [Envelope Builder Component](#envelope-builder-component).

<a name="BatchContentMessageStructure">![Batch Content Message Structure][batch.content.message]</a>

### Envelope Builder Component

The `BizTalk.Factory.Batching.RL1.Batch.Content.WCF-SQL.XML` receive location is relying on the `Be.Stateless.BizTalk.MicroComponent.EnvelopeBuilder` micro component. The purpose of this micro component it to apply a _generic_ `XSLT` transform on the batch content message returned from the database in order to convert it into an instance document of the expected envelope schema.

At first sight, applying a generic `XSLT` might seem impossible as there will certainly be a variety of envelope schemas, probably very different from one another. In order to do so, the `EnvelopeBuilder` micro component relies on composite multi-part message similar to the `XML` excerpt that follows &mdash;for which, by the way, there is no corresponding message schema deployed into Microsoft BizTalk Server®.

```XML
<agg:Root xmlns:agg="http://schemas.microsoft.com/BizTalk/2003/aggschema">
  <agg:InputMessagePart_0>
    <ns0:Envelope xmlns:ns0="urn:schemas.stateless.be:biztalk:envelope:2013:07">
      <ns:parts-here xmlns:ns="urn:schemas.stateless.be:biztalk:batch:2012:12" />
    </ns0:Envelope>
  </agg:InputMessagePart_0>
  <agg:InputMessagePart_1>
    <ns:BatchContent xmlns:ns="urn:schemas.stateless.be:biztalk:batch:2012:12">
      <ns:EnvelopeSpecName>...</ns:EnvelopeSpecName>
      <ns:Partition>...</ns:Partition>
      <ns:Parts>
        ...
      </ns:Parts>
    </ns:BatchContent>
  </agg:InputMessagePart_1>
</agg:Root>
```

This composite multi-part `XML` exhibits a couple of key characteristics that will allow a generic `XSLT` to be applied, no matter what is the expected envelope schema. Primarily, the `agg:InputMessagePart_0` element will always contain a dummy message that is an instance of the expected envelope schema and the `agg:InputMessagePart_1` element will always contain the batch content message as returned from the database. Furthermore, the dummy envelope instance message will always contain a placeholder —i.e. the `parts-here` element at the envelope schema’s `BodyXPath` expression— that has to be replaced with the verbatim content of the inner `XML` of the `agg:InputMessagePart_1/ns:BatchContent/ns:Parts` element.

### `EnvelopeMapSpecName` Envelope Schema Annotation

At times, the envelope message just built and submitted to the message box will immediately undergo another `XSLT` transformation on the part of its subscriber. To avoid two transformations in a row, it is possible to instruct the `EnvelopeBuilder` micro component to apply a custom `XSLT` stylesheet on the composite multi-part message. One simply has to annotate the target envelope schema with an `EnvelopeMapSpecName` instruction denoting the fully qualified name of the custom `XSLT` transform to apply, as in the following excerpt.

```XML
<xs:schema targetNamespace="..." xmlns:xs="http://www.w3.org/2001/XMLSchema"
           xmlns:san="urn:schemas.stateless.be:biztalk:annotations:2013:01">
  <xs:element name='Envelope'>
    <xs:annotation>
      <xs:appinfo>
        <san:EnvelopeMapSpecName>Be.Stateless.BizTalk.Unit.Transform.IdentityTransform, Be.Stateless.BizTalk.Unit, Version=1.0.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14</san:EnvelopeMapSpecName>
        ...
      </xs:appinfo>
    </xs:annotation>
    ...
  </xs:element>
</xs:schema>
```

> **Note.** To build the composite multi-part message, the micro pipeline component relies on an instance of the `Be.Stateless.BizTalk.Stream.CompositeStream` class whose content will be lazily &mdash;i.e. on demand while being read&mdash; constructed without any memory overhead.

### Envelope Message Publishing

Ultimately, the envelope message that is received by the `BizTalk.Factory.Batching.RL1.Batch.Content.WCF-SQL.XML` receive location and comes out of the `Be.Stateless.BizTalk.MicroComponent.EnvelopeBuilder` micro component is published to the message box. To better allow the interested parties to subscribe to this envelope message, its partition has been promoted into context, via the `Batch.EnvelopePartition` context property, on top of the message type, via the `BTS.MessageType` context property, as usual.

### Data Model Overview

<a name="BatchingApplicationDataModel">![Batching Application Data Model Overview][data.model]</a>

The preceding diagram illustrates the main database objects underlying the `BizTalk Factory`'s `Batching Application`. Unsurprisingly, the envelope schemas, represented by the `batch_Envelopes` table, are central in the data model and every other feature is related to them. The batch items, or parts, that are stored in the `batch_Parts` table, have to unequivocally relate to one envelope, which ultimately stands for an envelope schema, i.e. an `EnvelopeSpecName`. Similarly, the release policy definitions, represented by the `batch_ReleasePolicyDefinitions` table, are also individually linked to an envelope schema. Even the queueing/scheduling of batch releases consequent to the reception of control messages, represented by the `batch_QueuedControlledReleases` table, are linked to an envelope schema. The diagram also exhibits that the partition defaults to `0` and is thus a truly optional feature. Notice however that partition is a free text string in all of the `batch_Parts`, `batch_ReleasePolicyDefinitions`, and `batch_QueuedControlledReleases` tables; it is therefore the developer’s responsibility to guarantee that partition names will be consistent across all the three tables.

Looking back at [Batching Application Design Overview](#BatchingApplicationDesignOverview), one can see that the Microsoft BizTalk Server® artifacts are not directly interacting with the database tables, but only with some view and stored procedures. These stored procedures &mdash;namely `usp_batch_AddPart`, `usp_batch_QueueControlledRelease`, and `usp_batch_ReleaseNextBatch`,&mdash; which are not depicted on the diagram, are rather self-explanatory. The `vw_batch_ReleasePolicies` and `vw_batch_NextAvailableBatch` views, however, deserve some explanation.

The `vw_batch_ReleasePolicies` view evaluates the release policy definitions and shows their results, i.e. the list of every batch &mdash;denoted by an `EnvelopeSpecName` and `Partition`&mdash; that satisfies its policy definition predicates. Notice that for the sake of scalability and throughput, and at the expense of consistency, this view does not acquire any database locks.

The `vw_batch_NextAvailableBatch` view, together with the `usp_batch_ReleaseNextBatch` stored procedure, is used by the polling receive location to receive batches and publish envelope messages to the message box. This view integrates both the results of the previously mentioned `vw_batch_ReleasePolicies` view and the data of the `batch_QueuedControlledReleases` table &mdash;i.e. the batches scheduled for release consequent to the reception of control messages&mdash; to determine what will be the next batch to release, or alternatively, what will be the next envelope message to publish. This view and its partnering stored procedure have been designed for consistency and correctness; they do consequently acquire database locks, at the expense of scalability and throughput, though great care has been taken to limit the impact as much as possible.

> **Caution!** As the `vw_batch_NextAvailableBatch` view acquires database locks, it should not be used interactively, not even for operational or administrative purposes. To circumvent this shortcoming, should an operator agent still be willing to peek into the inner workings of the `Batching Application`, the `vw_batch_AvailableBatches` view has been created. This view offers a similar and even richer functionality than the `vw_batch_NextAvailableBatch` view &mdash;it lists all the batches that are ready to be released and not only the first one,&mdash; but without acquiring any lock and, of course, at the expense of consistency.

### Batch Registration

In order to be able to accumulate batch items for a given batch, one has first to register it. A batch, denoted by an `EnvelopeSpecName` and `Partition`, can be registered via the `usp_batch_Register` stored procedure, which should typically be called at deployment time. This stored procedure can moreover be used to configure the release policy of the batch being registered, as its signature shows:

```SQL
PROCEDURE [dbo].[usp_batch_Register]
   @envelopeSpecName nvarchar(256),
   @partition nvarchar(128) = '0',
   @enabled bit,
   @releaseOnElapsedTimeOut int = null,
   @releaseOnIdleTimeOut int = null,
   @releaseOnItemCount int = null,
   @enforceItemCountLimitOnRelease bit = 0
AS
```

Conversely, there is the `usp_batch_Unregister` stored procedure that should be called at undeployment time so as to unregister a batch and its release policy.

```SQL
PROCEDURE [dbo].[usp_batch_Unregister]
   @envelopeSpecName nvarchar(256),
   @partition nvarchar(128) = '0'
AS
```

<!-- TODO
Environment Tag
-->

<!-- TODO
## Installation

(https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Batching.Application) add-on application, whose [package](https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Batching.Application/releases/latest/download/Be.Stateless.BizTalk.Factory.Batching.Application.Deployment.zip) needs to be deployed as a full-fledged Microsoft BizTalk Server® application. This application relies on both `BizTalk.Factory` main and `BizTalk.Factory.Tracking` applications and generally needs to be referenced by any Microsoft BizTalk Server® applications that relies on any of its features
-->

<!-- TODO
### Environment Settings Overrides
-->

<!-- TODO
## Batching Application Activity Monitoring
-->

## Developer Help

Detailed developer help has been provided as `XML` comments directly embedded in source code. Though developers usually browse through this documentation while developing thanks to, for instance, JetBrains [ReSharper][resharper] quick help &mdash;<kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>F1</kbd>, an online version of this inlined help has also been provided here for greater reachability:

[![][help.badge]][help]

[![][help.schemas.badge]][help.schemas]

[![][help.maps.badge]][help.maps]

[![][help.unit.badge]][help.unit]

<!-- badges -->

[doc.main.badge]: https://img.shields.io/static/v1?label=BizTalk.Factory%20SDK&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.main]: https://www.stateless.be/ "BizTalk.Factory SDK User's Guide"
[doc.this.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Factory.Batching.Application&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.this]: https://www.stateless.be/BizTalk/Factory/Batching/Application "Be.Stateless.BizTalk.Factory.Batching.Application User's Guide"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.BizTalk.Pipelines&logo=github
[github]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipelines "Be.Stateless.BizTalk.Pipelines GitHub Repository"
[help.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Batching&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/Batching/README.md "Be.Stateless.BizTalk.Batching Developer Help"
[help.maps.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Batching.Maps&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help.maps]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/Batching/Maps/README.md "Be.Stateless.BizTalk.Batching.Maps Developer Help"
[help.schemas.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Batching.Schemas&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help.schemas]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/Batching/Schemas/README.md "Be.Stateless.BizTalk.Batching.Schemas Developer Help"
[help.unit.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Batching.Unit&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help.unit]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/BizTalk/Batching/Unit/README.md "Be.Stateless.BizTalk.Batching.Unit Developer Help"
[nuget.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Batching.svg?label=Be.Stateless.BizTalk.Batching&style=flat&logo=nuget
[nuget]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Batching "Be.Stateless.BizTalk.Batching NuGet Package"
[nuget.maps.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Batching.Maps.svg?label=Be.Stateless.BizTalk.Batching.Maps&style=flat&logo=nuget
[nuget.maps]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Batching.Maps "Be.Stateless.BizTalk.Batching.Maps NuGet Package"
[nuget.schemas.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Batching.Schemas.svg?label=Be.Stateless.BizTalk.Batching.Schemas&style=flat&logo=nuget
[nuget.schemas]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Batching.Schemas "Be.Stateless.BizTalk.Batching.Schemas NuGet Package"
[nuget.unit.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Batching.Unit.svg?label=Be.Stateless.BizTalk.Batching.Unit&style=flat&logo=nuget
[nuget.unit]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Batching.Unit "Be.Stateless.BizTalk.Batching.Unit NuGet Package"
[nuget.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/Be.Stateless.BizTalk.Batching?logo=nuget
[nuget.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=Be.Stateless.BizTalk.Batching&protocolType=NuGet "Be.Stateless.BizTalk.Batching Preview NuGet Package"
[nuget.maps.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/Be.Stateless.BizTalk.Batching.Maps?logo=nuget
[nuget.maps.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=Be.Stateless.BizTalk.Batching.Maps&protocolType=NuGet "Be.Stateless.BizTalk.Batching.Maps Preview NuGet Package"
[nuget.schemas.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/Be.Stateless.BizTalk.Batching.Schemas?logo=nuget
[nuget.schemas.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=Be.Stateless.BizTalk.Batching.Schemas&protocolType=NuGet "Be.Stateless.BizTalk.Batching.Schemas Preview NuGet Package"
[nuget.unit.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/Be.Stateless.BizTalk.Batching.Unit?logo=nuget
[nuget.unit.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=Be.Stateless.BizTalk.Batching.Unit&protocolType=NuGet "Be.Stateless.BizTalk.Batching.Unit Preview NuGet Package"
[package.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.Factory.Batching.Application?label=Be.Stateless.BizTalk.Factory.Batching.Application.Deployment.zip&style=flat&logo=github
[package]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Batching.Application/releases/latest/download/Be.Stateless.BizTalk.Factory.Batching.Application.Deployment.zip "Be.Stateless.BizTalk.Factory.Batching.Application Deployment Package"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Factory.Batching.Application%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=94&branchName=master "Be.Stateless.BizTalk.Factory.Batching.Application Continuous Integration Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Factory.Batching.Application%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=95&branchName=master "Be.Stateless.BizTalk.Factory.Batching.Application Manual Release Build Pipeline"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.Factory.Batching.Application?label=Release&logo=github
[release]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Batching.Application/releases/latest "Be.Stateless.BizTalk.Factory.Batching.Application GitHub Release"

<!-- links -->

[resharper]: https://www.jetbrains.com/resharper/

<!-- diagrams  -->

[application.design]: https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/icraftsoftware/biztalk.factory.github.io/master/BizTalk/Factory/Batching/Application/Design.puml "Batching Application Design Overview"
[batch.content.message]: https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/icraftsoftware/biztalk.factory.github.io/master/BizTalk/Factory/Batching/Application/BatchConentMessage.puml "Batch Content Message Structure"
[batch.release.message]: https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/icraftsoftware/biztalk.factory.github.io/master/BizTalk/Factory/Batching/Application/BatchReleaseMessage.puml "Batch Release Control Message Structure"
[data.model]: https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/icraftsoftware/biztalk.factory.github.io/master/BizTalk/Factory/Batching/Application/DataModel.puml "Batching Application Data Model Overview"

<!--
cSpell:ignore appinfo biztalk debatching nvarchar undeployment
-->
