# Configuration Specification Command

> **Tip** For the `PowerShell` newbies, you can then get detailed help on an individual command via a `PowerShell` command similar to:
>
> ```PowerShell
> Get-Help -Name Merge-ConfigurationSpecification -Detailed
> ```

The `Dsl.Configuration` `PowerShell` module provides one single command to process `XML` configuration specification `DSL` files:

```PowerShell
Merge-ConfigurationSpecification -Path <string[]> [-ConfigurationFileResolver <IConfigurationFileResolverStrategy[]>] [-CreateBackup] [-CreateUndo] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

Where

- `Path` indicates the configuration specification `DSL` files to process &mdash;the target `XML` configuration files into which to merge are part of the specification too,&mdash; see [Configuration Specification `DSL`](#configuration-specification-dsl);

- `ConfigurationFileResolver` is an ordered list of object instances of classes implementing the [IConfigurationFileResolverStrategy][i-configuration-file-resolver-strategy] interface that will participate in the resolution of target configuration file monikers, see [Configuration File Monikers and Resolvers](#configuration-file-monikers-and-resolvers);

- `CreateBackup` indicates whether to perform a backup of each target `XML` configuration file before actually merging a configuration specification into it;

- `CreateUndo` indicates whether to generate, for each `XML` configuration file that is the target of a configuration specification, a reverse configuration specification capable of undoing all the modifications actually made.

> **Remark** No backup will be performed nor an undo specification generated should the merge of a configuration specification would not result in any changes to an `XML` configuration file.

## Configuration Specification `DSL`

The configuration specification `DSL` is an embedded `XML` `DSL`. As the following example illustrates, a configuration specification deceptively looks like an actual `XML` configuration file:

```xml
<configuration xmlns:config="urn:schemas.stateless.be:dsl:configuration:annotations:2020"
               config:targetConfigurationFiles="global:clr4:machine.config">
  <system.serviceModel>
    <extensions>
      <behaviorExtensions>
        <add
          name="propertyPropagator"
          type="Be.Stateless.BizTalk.ServiceModel.Configuration.PropertyPropagationBehaviorExtension, Be.Stateless.BizTalk.ServiceModel, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14"
          config:operation="insert"
          config:key="name" />
      </behaviorExtensions>
    </extensions>
  </system.serviceModel>
  <system.web>
    <applicationPool
      maxConcurrentRequestsPerCPU="5000"
      maxConcurrentThreadsPerCPU="0"
      requestQueueLimit="5000"
      config:operation="update"
      config:key="name"
      config:scrap="maxConcurrentThreadsPerCPU, requestQueueLimit" />
  </system.web>
</configuration>
```

What distinguishes a configuration specification from an actual `XML` configuration lies in the following attributes:

- The `XML` namespace declaration attribute for `urn:schemas.stateless.be:dsl:configuration:annotations:2020`, which is required by the other `DSL` attributes. This attribute is not required per se, but not declaring it would hide away any `DSL` attribute from the `DSL` processing engine;

  > **Remark** The namespace prefix `config` is irrelevant and left to the developer's discretion.

- The mandatory `targetConfigurationFiles` attribute, which is a coma-separated list of target `XML` configuration file monikers, see [Configuration File Monikers and Resolvers](#configuration-file-monikers-and-resolvers);

- The optional `operation` attribute &mdash;`action` is a supported alias,&mdash; which indicates what operation this annotated specification element must undergo to be merged into the targeted `XML` configuration files. The `operation` may have any single of the following values:

  - `insert`, which indicates that this annotated specification element, together with its attributes, should be inserted into the targeted `XML` configuration files;

  - `update`, which indicates that the attributes of this annotated specification element should be merged &mdash;adding new ones or updating existing ones&mdash; into the attributes of the configuration element that corresponds to this specification element in the targeted `XML` configuration files;

  - `upsert`, which indicates that this annotated specification element should either be used to update the targeted `XML` configuration files should a corresponding configuration element be found, or be inserted into otherwise;

  - `delete`, which indicates that the configuration element corresponding to this annotated specification element should be deleted, altogether with its attributes and child elements;

  - `none`, which indicates that the configuration element corresponding to this annotated specification element should be used as a simple pivot element, without undergoing any alteration, so as to preserve the document ordering existing among the siblings of this specification element when merging them into the targeted `XML` configuration files.
    > **Remark** The document ordering of the specification elements will always be preserved during their merge into the targeted `XML` configuration files.

- The optional `key` attribute &mdash;`discriminant` is a supported alias,&mdash; which is a coma-separated list of attribute names denoting the set of attributes, together with their values, that will be used in addition to the path and name of this annotated specification element to find a corresponding element in the targeted `XML` configuration files;

- The optional `scrap` attribute, which can only be used in conjunction with an `update` operation and is a coma-separated list of the names of the attributes that should be deleted when merging this annotated specification element.

> **Remark** The annotation attributes which are specific to the configuration specification `DSL` are naturally left off during the processing of a specification and not merged into the targeted `XML` configuration files.

### Configuration Specification Idempotence

Configuration specification are idempotent, in the sense that if a specification has already been successfully processed &mdash;i.e. merged into its target `XML` configuration files,&mdash; it should not fail if its processing is triggered again. In other word, if an `XML` configuration file has already undergone the successful merge of a configuration specification, this `XML` configuration file will not be altered in any new way should the same configuration specification be merged into again.

To that end, each operation defines and implements its own preserving notion of idempotency. Details about the algorithm applied during the merge of a configuration specification for each of the operations is given by the developer help of the [`ConfigurationElement.Apply'][configuration-element-apply] method, but roughly speaking, each operation behave according to the following principles:

- The `insert` operation will succeed if one or no configuration element equivalent to the specification one is found, but will fail otherwise;

- The `update` operation will succeed if one configuration element corresponding or equivalent to the specification one is found, but will fail otherwise;

- The `upsert` operation will succeed if any of its `insert` or `update` variant will succeed, but will fail otherwise;

- The `delete` operation will succeed if one or no configuration element equivalent to the specification one is found, but will fail otherwise.

> **Remark** A configuration element is said to **correspond** to its specification element when both have the same name and both are located at the same relative place in their own respective `XML` infoset &mdash;in other words, when both elements have the same `XPath` location,&mdash;see [`SpecificationElement.IsSatisfiedBy`][specification-element-issatisfiedby] method. \
> A configuration element is said to be **equivalent** to its specification element when it corresponds to this specification element and that for each of the specification attributes there is an configuration attribute having both the same name and value. By default, all the specified attributes are taken into account for determining the equivalence of the elements, but only those attributes listed in the `key` annotation are taken into account should this annotation be specified, see [`SpecificationElement.IsEquatedBy`][specification-element-isequatedby] method.

## Configuration File Monikers and Resolvers

The `Dsl.Configuration` `PowerShell` module provides two implementations of the [IConfigurationFileResolverStrategy][i-configuration-file-resolver-strategy] interface:

- [ConfigurationFileResolverStrategy][configuration-file-resolver-strategy], which can resolve traditional file paths, provided the files exist on disk, e.g. `C:\Windows\Microsoft.NET\Framework64\v4.0.30319\Config\machine.config`;

- [ClrConfigurationFileResolverStrategy][clr-configuration-file-resolver-strategy], which can resolve `XML` configuration files monikers of the form `global:clr?:[<32bits|64bits>:]<machine|web>.config`, that is to say `.NET`'s global `XML` configuration files; e.g. `global:clr4:machine.config` would resolve to both 32 and 64 bits global machine.config files for the `CLR` 4, while `global:clr2:32bits:web.config` would resolve to the 32 bit global web.config of the `CLR` 2.

The `Dsl.Configuration` `PowerShell` module will _always_ append these two resolvers, [ClrConfigurationFileResolverStrategy][clr-configuration-file-resolver-strategy] and [ConfigurationFileResolverStrategy][configuration-file-resolver-strategy], in _that order_, to the list of custom object instances passed as arguments to the `ConfigurationFileResolver` command parameter.

When used throughout the `BizTalk.Deployment` `PowerShell` module, a third implementation of the [IConfigurationFileResolverStrategy][i-configuration-file-resolver-strategy] interface is always added before the preceding two resolvers:

- [BizTalkConfigurationFileResolverStrategy][biztalk-configuration-file-resolver-strategy], which can resolve `XML` configuration files monikers of the form `global:[<32bits|64bits>:]biztalk.config`, that is to say Microsoft BizTalk Server®'s global `XML` configuration files; e.g. `global:64bits:biztalk.config` would resolve to 64 bits configuration file `C:\Program Files (x86)\Microsoft BizTalk Server\BTSNTSvc64.exe.config`, while `global:biztalk.config` would resolve to both 32 and 64 bits configuration files.

Given that ordered list of custom and built-in `XML` configuration file moniker resolvers, the processing engine will only use the _first_ resolver in this ordered list that can resolve a configuration file moniker and all the subsequent resolvers in the list will be ignored.

<!-- links -->

[biztalk-configuration-file-resolver-strategy]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment/blob/master/src/Be.Stateless.BizTalk.Deployment.Cmdlets/Dsl/Configuration/Resolvers/BizTalkConfigurationFileResolverStrategy.cs
[clr-configuration-file-resolver-strategy]: https://github.com/icraftsoftware/Be.Stateless.Dsl.Configuration/blob/master/src/Be.Stateless.Dsl.Configuration/Dsl/Configuration/Resolver/ClrConfigurationFileResolverStrategy.cs
[configuration-element-apply]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/Dsl/Configuration/ConfigurationElement.Apply(SpecificationElement).md#configurationelementapplyspecificationelement-method
[configuration-file-resolver-strategy]: https://github.com/icraftsoftware/Be.Stateless.Dsl.Configuration/blob/master/src/Be.Stateless.Dsl.Configuration/Dsl/Configuration/Resolver/ConfigurationFileResolverStrategy.cs
[i-configuration-file-resolver-strategy]: https://github.com/icraftsoftware/Be.Stateless.Dsl.Configuration/blob/master/src/Be.Stateless.Dsl.Configuration/Dsl/Configuration/Resolver/IConfigurationFileResolverStrategy.cs
[specification-element-isequatedby]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/Dsl/Configuration/SpecificationElement.IsEquatedBy(ConfigurationElement).md#specificationelementisequatedbyconfigurationelement-method
[specification-element-issatisfiedby]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/Dsl/Configuration/SpecificationElement.IsSatisfiedBy(ConfigurationElement).md#specificationelementissatisfiedbyconfigurationelement-method

<!--
cSpell:ignore biztalk BTSNTSvc idempotence idempotency infoset minifier upsert
-->
