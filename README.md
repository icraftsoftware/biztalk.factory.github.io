# BizTalk.Factory Overview

`BizTalk.Factory` 2.0 is both a Microsoft BizTalk Server® 2020 software development kit and a declarative Microsoft BizTalk Server® 2020 deployment framework.

They are many other available Microsoft BizTalk Server® extensions that try to fill the gap and provide some decent development and deployment experiences, for instance [BizTalk Server Open Source Community](https://github.com/BizTalkCommunity), [BizTalk Deployment Framework](https://github.com/BTDF/DeploymentFramework), [BizTalk Server Pipeline Component Wizard](https://github.com/plykkegaard/btsplcw), [BizTalk Software Factory](https://github.com/jeanpaulsmit/BizTalk-Software-Factory) (not to be confused with `BizTalk.Factory` itself), Eliasen's [BizTalk Pipeline Components](http://biztalk.eliasen.dk/Pipelines.aspx), and so on...

`BizTalk.Factory` is however far more reaching and cohesive in its unique and distinctive approach: instead of being based on, or leveraging, designer surfaces or wizards, it strives to provide a code centric, or code-first, development experience. Wherever possible, `BizTalk.Factory` will offer a `C#` fluent API to replace the designer surface. This is noticeably the case to what concerns [Pipelines](./BizTalk/Dsl/Pipeline/README.md), [Bindings](./BizTalk/Dsl/Binding/README.md), and [Rule Programs](./BizTalk/Dsl/Rule/README.md).

`BizTalk.Factory` will not try to replace the Microsoft BizTalk Server® orchestration designer surface though, but it provides nonetheless an alternative by leveraging custom pipelines and custom pipeline components to provide a development experience where orchestration-based flows are implemented by messaging-only, or publish-subscribe, flows for the simple reason that messaging-only flows are generally easier to maintain &mdash;whether it is development or testing,&mdash; simpler to deploy, and more efficient performance-wise.

`BizTalk.Factory` consists of three different sorts of components and packages:

- The _runtime_ ones, which are made up of .NET assemblies, Microsoft BizTalk Server® applications and Microsoft SQL Server® databases. They must priorly be installed on every server belonging to a Microsoft BizTalk Server® group in order to be able to run Microsoft BizTalk Server® applications relying on the `BizTalk.Factory` SDK. All the `BizTalk.Factory` runtime's deployment packages are available as GitHub assets in their various repository, see [Runtime Packages](./README.md#runtime-packages);

- The _deployment_ ones, which are made up of a series of Microsoft PowerShell® modules. They must be installed on every server belonging to a Microsoft BizTalk Server® group in order to be able to install the `BizTalk.Factory` SDK's runtime packages and any custom Microsoft BizTalk Server® application built on top. All the Microsoft PowerShell® modules are available on [PowerShell Gallery][powershell.gallery.icraftsoftware], see [Deployment Packages](./README.md#deployment-packages);

- The _development_ ones, which are made up of plain .NET assemblies. Referencing these assemblies is obviously required during development, but they must not be installed per se. For this reason, all these assemblies are made available on [NuGet][nuget.icraftsoftware], see [Development Packages](./README.md#development-packages).

## Runtime Packages

`BizTalk.Factory` runtime packages consist of the following packages:

- [BizTalk.Factory Runtime](./BizTalk/Factory/Runtime/README.md) is a Microsoft BizTalk Server® runtime made of .NET assemblies that can be deployed without any Microsoft BizTalk Server® footprint; it merely requires assemblies to be GAC-deployed and global configuration files to be edited. Notice that since this package has no Microsoft BizTalk Server® footprint, it can be patched or even fully redeployed at any time without any other impact on the Microsoft BizTalk Server® group than a small down time while restarting the host instances;

- [BizTalk.Factory Application](./BizTalk/Factory/Application/README.md) is a scaffolding Microsoft BizTalk Server® application, similarly to the built-in `BizTalk.System` application. `BizTalk.Factory` Application has been built somehow as an _empty shell_ consisting of a few general purpose Microsoft BizTalk Server® artifacts (i.e. context properties, pipeline components, pipelines, and schemas) that delegate the vast majority of their work to the `BizTalk.Factory` Runtime. This package consequently should almost never need to be patched or even redeployed and can therefore be relied upon and referenced by any other Microsoft BizTalk Server® applications without major deployment concern. Among the many features this application offers, the [micro-pipelines](./BizTalk/Pipelines/README.md) are probably the most valuable;

- A [BizTalk.Factory.Activity.Tracking Application](./BizTalk/Factory/Activity/Tracking/Application/README.md) add-on application that requires to be deployed as a full-fledged Microsoft BizTalk Server® application. This application relies on the main `BizTalk.Factory` Application but does not need to be referenced by any other Microsoft BizTalk Server® 2020 applications, should they even rely on any of its features;

- A [BizTalk.Factory.Batching Application](./BizTalk/Factory/Batching/Application/README.md) add-on application that requires to be deployed as a full-fledged Microsoft BizTalk Server® application. This application relies on both `BizTalk.Factory` and `BizTalk.Factory.Tracking` Applications and generally needs to be referenced by any Microsoft BizTalk Server® application that relies on any of its features.

> **Remark** To develop and even _unit_ test any Microsoft BizTalk Server® artifacts, none of these packages needs to be deployed as all of the required .NET assemblies to write code against are publicly available on [NuGet][nuget.icraftsoftware].
>
> Running the automated system tests of messaging-only or orchestration-based flows is the exception to the rule and requires these packages to be deployed.

## Deployment Packages

`BizTalk.Factory` deployment packages consist of the following Microsoft PowerShell® modules, which have been made publicly available on [PowerShell Gallery][powershell.gallery.icraftsoftware] &mdash;altogether they provide a declarative deployment framework suited for Microsoft BizTalk Server® 2020:

- [BizTalk.Administration](./PowerShell/Module/BizTalk/Administration/README.md), which is a `PowerShell` utility module providing commands to administrate, configure, and explore Microsoft BizTalk Server® and its artifacts;

- [BizTalk.Deployment](./PowerShell/Module/BizTalk/Deployment/README.md), which is an extensible `PowerShell` utility module based on a deployment framework featuring a declarative resource-driven task model and providing commands to deploy full-fledged Microsoft BizTalk Server® applications;

- [Dsl.Configuration](./PowerShell/Module/Dsl/Configuration/README.md), which is a `PowerShell` utility module providing an embedded `XML` `DSL` to create configuration file specifications and commands to edit `XML` configuration files;

- [Exec](./PowerShell/Module/Exec/README.md), which is a `PowerShell` utility module providing commands to work with external executables;

- [Resource.Manifest](./PowerShell/Module/Resource/Manifest/README.md), which is a `PowerShell` module providing commands to define resource manifests made of resource groups &mdash;i.e. resources grouped by kind. Resource manifests are declarative Microsoft BizTalk Server® deployment recipes that can be entrusted to the [BizTalk.Deployment](./PowerShell/Module/BizTalk/Deployment/README.md) `PowerShell` module, which will take care of the actual deployment;

- [Psx](./PowerShell/Module/Psx/README.md), which is a general scaffolding `PowerShell` utility module.

## Development Packages

> **Tips** All the `BizTalk.Factory` `NuGet` packages are [Source Link][source-link]-enabled for an immersive debugging experience.

The development packages consist of plain `.NET` assemblies that have been made available on [NuGet][nuget.icraftsoftware]. According to their purpose, these assemblies, which naturally have to be referenced at development time, fall into several categories:

- The ones that provide core runtime functionalities. These assemblies usually do not require to be installed on a development box unless the developer needs to run Microsoft BizTalk Server® applications relying on them (e.g. to execute the automated tests of messaging-only or orchestration-based flows). If necessary, they should be deployed along with the [Runtime Packages](./README.md#runtime-packages);

- The ones that provide embedded `C#` [DSL][dsl]s as a replacement to Microsoft BizTalk Server® designer surfaces &mdash;see [Pipeline DSL](./BizTalk/Dsl/Pipeline/README.md), and [Rule DSL](./BizTalk/Dsl/Rule/README.md)&mdash; or as a code-first/fluent alternative to the configuration of Microsoft BizTalk Server® applications &mdash;see [Binding DSL](./BizTalk/Dsl/Binding/README.md). These assemblies must never be deployed and are made available as `NuGet` packages only;

- The ones that provide custom `MSBuild` tasks leveraging the artifacts written in either one of the `BizTalk.Factory`'s `DSL`s; see [Be.Stateless.BizTalk.Build.Tasks](./BizTalk/Build/Tasks/README.md). The `Be.Stateless.BizTalk.Build.Tasks` assembly however provides only the `MSBuild` tasks, to actually integrate them into the `MSBuild` process, the developer has to reference the [BizTalk.Server.2020.Build][biztalk.server.2020.build] package, which tailors the `MSBuild` process to Microsoft BizTalk Server® 2020;

- The ones to be used as complementary unit test libraries helping the developers to unit test code written on top of `BizTalk.Factory` SDK. Some of these unit testing library assemblies even come in separate flavors, leveraging either or both [NUnit](https://nunit.org/) and [xUnit](https://xunit.net/) testing frameworks. These assemblies are obviously only required at development time and are made available as `NuGet` packages only &mdash;look for [Be.Stateless.\*.Unit](https://www.nuget.org/packages?q=be.stateless.*.unit), [Be.Stateless.\*.NUnit](https://www.nuget.org/packages?q=be.stateless.*.nunit), and [Be.Stateless.\*.XUnit](https://www.nuget.org/packages?q=be.stateless.*.xunit) `NuGet` packages. These assemblies must never be deployed.

> **Caution!** Both [BizTalk.Server.2020.Build][biztalk.server.2020.build] `NuGet` package and [BizTalk.Deployment](./PowerShell/Module/BizTalk/Deployment/README.md) `PowerShell` module's accompanying runtime and `DSL` assemblies must be version aligned. The developer should therefore take care that the versions of the assemblies referenced in his projects are compatible with the one coming with either [BizTalk.Server.2020.Build][biztalk.server.2020.build] or [BizTalk.Deployment](./PowerShell/Module/BizTalk/Deployment/README.md).

## Installing BizTalk.Factory

<!-- TODO -->

## Building BizTalk.Factory

<!-- TODO -->

<!-- links -->

[biztalk.server.2020.build]: https://www.nuget.org/packages/BizTalk.Server.2020.Build
[dsl]: https://en.wikipedia.org/wiki/Domain-specific_language "Domain-Specific Language"
[nuget.icraftsoftware]: https://www.nuget.org/profiles/icraftsoftware
[powershell.gallery.icraftsoftware]: https://www.powershellgallery.com/profiles/icraftsoftware
[source-link]: https://docs.microsoft.com/en-us/dotnet/standard/library-guidance/sourcelink

<!--
cSpell:ignore Eliasen priorly
-->
