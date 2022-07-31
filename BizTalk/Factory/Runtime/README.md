# BizTalk.Factory Runtime

[![][github.badge]][github]

##### Build Pipelines

[![][pipeline.mr.badge]][pipeline.mr]

[![][pipeline.ci.badge]][pipeline.ci]

##### Latest Release

[![][package.badge]][package]

[![][release.badge]][release]

##### Release Preview

<!-- TODO preview deployment packages -->

## Overview

Deployment package for `BizTalk.Factory` Runtime, which is part of the larger [BizTalk.Factory](../../../README.md) SDK. This package is made of the following .NET components:

- [Be.Stateless.Extensions](../../../Extensions/README.md), which provides general purpose utility classes and extension methods for various .NET types;

- [Be.Stateless.Reflection](../../../Reflection/README.md), which provides assembly loader and reflection helper methods for general purpose .NET development that eases the rare occasions on which you have no other choice than to invoke methods via reflection or tap into the assembly loading process;

- [Be.Stateless.Runtime](../../../Runtime/README.md), which provides service injection at startup time of any .NET Framework managed process and caching abstractions;

- [Be.Stateless.Security](../../../Security/README.md), which provides a security helper class allowing to impersonate a Windows identity when invoking a .NET `delegate`;

- [Be.Stateless.Stream](../../../Stream/README.md), which provides a stream class library for general purpose .NET development;

- [Be.Stateless.Xml](../../../Xml/README.md), which provides an `XML` class library for general purpose .NET development;

- [Be.Stateless.BizTalk.Abstractions](../../Abstractions/README.md), which provides various abstractions over Microsoft BizTalk Server®'s message contexts and context properties;

- [Be.Stateless.BizTalk.Messaging](../../Messaging/README.md), which provides a pipeline-centric messaging class library for general purpose Microsoft BizTalk Server® development;

- [Be.Stateless.BizTalk.Pipeline.MicroComponents](../../Pipeline/MicroComponents/README.md), which provides various general purpose micro components meant to be run by the `BizTalk.Factory`'s [MicroPipelineComponent][micro-pipeline-component] &mdash;see [Be.Stateless.BizTalk.Pipeline.Components](./../../Pipeline/Components/README.md), [Be.Stateless.BizTalk.Pipelines](./../../Pipelines/README.md), [Be.Stateless.BizTalk.Dsl.Pipeline](./../../Dsl/Pipeline/README.md), and [Be.Stateless.BizTalk.Dsl.Binding](./../../Dsl/Binding/README.md) for more information about micro pipelines;

- [Be.Stateless.BizTalk.ServiceModel](../../ServiceModel/README.md), which provides both `WCF` behavior extensions dedicated to Microsoft BizTalk Server®, and utility classes allowing to compose `WCF` relays using Microsoft BizTalk Server® schema and map artifacts;

- [Be.Stateless.BizTalk.Settings](../../Settings/README.md), which provides a streamlined `API` over the native, awkward to use, Microsoft BizTalk Server® Enterprise Single Sign-On `API`, the main purpose of which is to allow to easily store Microsoft BizTalk Server® dynamic configuration settings right into `SSO` configuration stores instead of configuration files scattered across servers;

- [Be.Stateless.BizTalk.Stream](../../Stream/README.md), which provides a stream class library for general purpose Microsoft BizTalk Server® development;

- [Be.Stateless.BizTalk.Transform.ExtensionObjects](../../Transforms/README.md), which provides a transform class library for general purpose Microsoft BizTalk Server® development.;

- [Be.Stateless.BizTalk.XLang](../../XLang/README.md), which provides an orchestration-centric messaging class library for general purpose Microsoft BizTalk Server® development;

- [Be.Stateless.BizTalk.Xml](../../Xml/README.md), which essentially is an `XML` class library for general purpose Microsoft BizTalk Server® development;

- [Be.Stateless.BizTalk.Factory.Logging][be.stateless.biztalk.factory.logging], which is a `BizTalk.Factory` Runtime's private component &mdash;i.e. not published as a `NuGet` package&mdash; that provides the [LoggingConfigurationLoader][logging-configuration-loader] service class which, once registered as an [IStartupService][i-startup-service], will ensure that `log4net` configuration is loaded when a Microsoft BizTalk Server® Host Instance starts.

> **Remark** The assemblies being named **Be.Stateless.BizTalk.\*** are assemblies depending on and made up for Microsoft BizTalk Server® and currently target the .NET Framework 4.8. The other assemblies are not tied to Microsoft BizTalk Server® and currently target multiple frameworks: .NET Standard 2.0, .NET Core 3.1, and .NET Framework 4.8.

## Component Model

The following component diagram shows a trimmed view of the components that are part of the `BizTalk.Factory Runtime` package where all transitive dependencies between components have been pruned.

![][component.diagram]

See this [alternate component diagram](./ComponentModel.md) for a comprehensive view of all the dependencies between the components.

## Installation

<!-- badges -->

[doc.main.badge]: https://img.shields.io/static/v1?label=BizTalk.Factory%20SDK&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.main]: https://www.stateless.be/ "BizTalk.Factory SDK User's Guide"
[doc.this.badge]: https://img.shields.io/static/v1?label=Be.Stateless.BizTalk.Factory.Runtime&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.this]: https://www.stateless.be/BizTalk/Factory/Runtime "Be.Stateless.BizTalk.Factory.Runtime User's Guide"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.BizTalk.Factory.Application&logo=github
[github]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Runtime "Be.Stateless.BizTalk.Factory.Runtime GitHub Repository"
[package.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.Factory.Runtime?label=Be.Stateless.BizTalk.Factory.Runtime.Deployment.zip&style=flat&logo=github
[package]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Runtime/releases/latest/download/Be.Stateless.BizTalk.Factory.Runtime.Deployment.zip "Be.Stateless.BizTalk.Factory.Runtime Deployment Package"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Factory.Runtime%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=88&branchName=master "Be.Stateless.BizTalk.Factory.Runtime Continuous Integration Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Factory.Runtime%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=89&branchName=master "Be.Stateless.BizTalk.Factory.Runtime Manual Release Build Pipeline"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.Factory.Runtime?label=Release&logo=github
[release]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Runtime/releases/latest "Be.Stateless.BizTalk.Factory.Runtime GitHub Release"

<!-- links -->

[be.stateless.biztalk.factory.logging]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Runtime/tree/master/src/Be.Stateless.BizTalk.Factory.Logging
[i-startup-service]: https://github.com/icraftsoftware/Be.Stateless.Runtime/blob/master/src/Be.Stateless.Runtime/Runtime/IStartupService.cs
[logging-configuration-loader]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Runtime/blob/master/src/Be.Stateless.BizTalk.Factory.Logging/Factory/Logging/LoggingConfigurationLoader.cs
[micro-pipeline-component]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Pipeline.Components/blob/master/src/Be.Stateless.BizTalk.Pipeline.Components/Component/MicroPipelineComponent.cs

<!-- diagrams  -->

[component.diagram]: https://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/icraftsoftware/biztalk.factory.github.io/master/BizTalk/Factory/Runtime/ComponentModel.Trimmed.puml "Component Diagram"

<!--
cSpell:ignore BTSNTSvc
-->
