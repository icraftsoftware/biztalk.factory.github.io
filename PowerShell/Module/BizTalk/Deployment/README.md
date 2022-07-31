# BizTalk.Deployment PowerShell Module

[![][github.badge]][github]

##### Build Pipelines

[![][pipeline.mr.badge]][pipeline.mr]

[![][pipeline.ci.badge]][pipeline.ci]

##### Latest Release

[![][module.badge]][module]

[![][release.badge]][release]

##### Release Preview

[![][module.preview.badge]][module.preview]

##### Documentation

[![][doc.main.badge]][doc.main]

[![][doc.this.badge]][doc.this]

## Overview

`BizTalk.Deployment` is an extensible `PowerShell` utility module based on a deployment framework featuring a declarative resource-driven task model and providing commands to deploy full-fledged Microsoft BizTalk Server® applications.

This module furthermore depends on the following third-party `PowerShell` Modules:

- [Gac](https://www.powershellgallery.com/packages/Gac);
- [InvokeBuild][invoke-build];
- [SqlServer](https://www.powershellgallery.com/packages/SqlServer).

## Rationale

Deploying a Microsoft BizTalk Server® application is often a complex and tedious task if one cannot comprehensively automate the process. Indeed there are generally much more going on than just deploying the Microsoft BizTalk Server® artifacts, it may be necessary to modify configuration files, to deploy Windows® services, to deploy custom databases or database objects, to register `COM+` service components, etc.

Microsoft BizTalk Server® offers a [`Windows Installer`][windows-installer]-based approach to produce `MSI` deployment packages as a way to deploy custom applications. `MSI` packages are however generally hard to produce and even harder to customize, especially since the way packages are produced by Microsoft BizTalk Server® is undocumented. For these reasons, the approach offered natively by Microsoft BizTalk Server® falls short from meeting all our needs and expectations.

As a better alternative, one could entrust the deployment of Microsoft BizTalk Server® applications to [BizTalk Deployment Framework](https://github.com/BTDF/DeploymentFramework), which, being built on top of `MSBuild`, is as extensible and customizable as `MSBuild` is. Thanks to its declarative and resource-driven task model, `MSBuild` is very appealing and quite easy to embrace. Customizing `MSBuild` however requires a dedicated skill set and, as such, is often a cumbersome and tedious process furthermore mixing different technologies &mdash;custom `MSBuild` tasks are generally written in `C#` while custom `MSBuild` targets are written in native `XML`-based `MSBuild` script. The [operational semantics][evaluation-phase] of `MSBuild` is also inherently quite complex and follows a multi-phase process. Custom [item group][evaluate-items] definitions are moreover often very delicate to get right.

While willing to keep the declarative and resource-driven task model that `MSBuild` offers, `BizTalk.Factory` departs from it for extensibility and customization reasons and choses to rely on `PowerShell` instead. `PowerShell` has tremendous stories of achievements and customizations, as essentially, nothing on the `Windows`® platform is beyond the reach of `PowerShell`, be it native commands, `WMI`, or even `.NET` libraries. Writing custom tasks is therefore quite easy to achieve in and with `PowerShell`.

`PowerShell` even natively supports a declarative and resource-driven task execution model thanks to its [`Desired State Configuration`][dsc] service. However the granularity of the _state_ that can be operated upon is too coarse &mdash;the whole computer&mdash; when one wants to individually un/deploy Microsoft BizTalk Server® applications. The user experience with `DSC` is moreover a little more involved than the usual [`REPL`][repl] `PowerShell` experience that `BizTalk.Factory` wanted to keep because it is more easily amenable to automation via Azure pipelines.

Alternative to `PowerShell` `DSC` therefore had to be found; more specifically, ways to provide both a declarative resource specification &mdash;a la `MSBuild`'s [`ItemGroup`][msbuild-item-group] or `DSC`'s [`DSCResource`][dsc-resource]&mdash; and a declarative task execution engine &mdash;a la `MSBuild`'s [`Target`][msbuild-targets] or `DSC`'s [resource methods][dsc-methods]. There are a few `PowerShell` modules that provide a declarative task execution engine &mdash;for instance [psake][psake] and [Invoke-Build][invoke-build]&mdash; and `BizTalk.Factory` has chosen to rely on [Invoke-Build][invoke-build]. There are however no `PowerShell` module that provides a declarative resource specification, and `BizTalk.Factory` has chosen to build its own, [Resource.Manifest](../../Resource/Manifest/README.md).

## Usages

`BizTalk.Deployment` provides three broad categories of functionalities. The first is provided by the top-level commands that allow to install or uninstall Microsoft BizTalk Server® applications. The secondary is twofold and provided by the commands that allows to consume code-first application bindings &mdash;see [Be.Stateless.BizTalk.Dsl.Binding](../../../../BizTalk/Dsl/Binding/README.md)&mdash; on the one hand, and the commands that allows to configure `SSO` affiliate applications and their configuration stores &mdash;see [Be.Stateless.BizTalk.Settings](../../../../BizTalk/Settings/README.md)&mdash; on the other hand. The third is provided by the deployment tasks whose execution will be entrusted to [Invoke-Build][invoke-build] on the basis of the resources declared in the deployment manifest &mdash;see [Resource.Manifest](../../Resource/Manifest/README.md).

- [Installing and Uninstalling Microsoft BizTalk Server® Applications and Libraries](./InstallationCommands.md);

- [Consuming Code-First Application Bindings](./ApplicationBindingCommands.md) and [Configuring SSO Affiliate Applications and Configuration Stores](./AffiliateApplicationCommands.md);

- [Deployment Tasks](./DeploymentTasks.md).

## Installation

In order to be able to install the `PowerShell` module, you might have to trust the `be.stateless`'s certificate public key beforehand; see these [instructions](../../Installation.md) for details on how to proceed.

<!-- badges -->

[doc.install]: https://www.stateless.be/PowerShell/Module/Installation.html "PowerShell Module Installation"
[doc.main.badge]: https://img.shields.io/static/v1?label=BizTalk.Factory%20SDK&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.main]: https://www.stateless.be/ "BizTalk.Factory SDK User's Guide"
[doc.this.badge]: https://img.shields.io/static/v1?label=BizTalk.Deployment&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.this]: https://www.stateless.be/PowerShell/Module/BizTalk/Deployment "BizTalk.Deployment PowerShell Module User's Guide"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.PowerShell.Module.BizTalk.Deployment&logo=github
[github]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment "Be.Stateless.PowerShell.Module.BizTalk.Deployment GitHub Repository"
[module.badge]: https://img.shields.io/powershellgallery/v/BizTalk.Deployment.svg?label=BizTalk.Deployment&style=flat&logo=powershell
[module]: https://www.powershellgallery.com/packages/BizTalk.Deployment "BizTalk.Deployment Module"
[module.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/BizTalk.Deployment?logo=powershell
[module.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=BizTalk.Deployment&protocolType=NuGet "BizTalk.Deployment PowerShell Module Preview"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.PowerShell.Module.BizTalk.Deployment%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=29&branchName=master "Be.Stateless.PowerShell.Module.BizTalk.Deployment Continuous Integration Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.PowerShell.Module.BizTalk.Deployment%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=30&branchName=master "Be.Stateless.PowerShell.Module.BizTalk.Deployment Manual Release Build Pipeline"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment?label=Release&logo=github
[release]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment/releases/latest "Be.Stateless.PowerShell.Module.BizTalk.Deployment Release"

<!-- links -->

[dsc-methods]: https://docs.microsoft.com/en-us/powershell/dsc/concepts/resources#implementing-the-methods
[dsc-resource]: https://docs.microsoft.com/en-us/powershell/dsc/concepts/resources#create-a-dscresource-powershell-class
[dsc]: https://docs.microsoft.com/en-us/powershell/dsc/overview
[evaluate-items]: https://docs.microsoft.com/en-us/visualstudio/msbuild/build-process-overview#evaluate-items
[evaluation-phase]: https://docs.microsoft.com/en-us/visualstudio/msbuild/build-process-overview#evaluation-phase
[invoke-build]: https://github.com/nightroman/Invoke-Build
[msbuild-item-group]: https://docs.microsoft.com/en-us/visualstudio/msbuild/itemgroup-element-msbuild
[msbuild-targets]: https://docs.microsoft.com/en-us/visualstudio/msbuild/msbuild-targets
[psake]: https://github.com/psake/psake
[repl]: https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop
[windows-installer]: https://docs.microsoft.com/en-us/windows/win32/msi/windows-installer-portal

<!--
cSpell:ignore psake
-->
