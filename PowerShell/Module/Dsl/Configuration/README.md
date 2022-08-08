# Dsl.Configuration PowerShell Module

[![][github.badge]][github]

##### Build Pipelines

[![][pipeline.mr.badge]][pipeline.mr]

[![][pipeline.ci.badge]][pipeline.ci]

##### Latest Release

[![][module.badge]][module]

[![][nuget.badge]][nuget]

[![][release.badge]][release]

##### Release Preview

[![][module.preview.badge]][module.preview]

[![][nuget.preview.badge]][nuget.preview]

## Overview

`Dsl.Configuration` is a `PowerShell` utility module providing commands to edit `XML` configuration files. These commands come in two flavours:

- The one allowing to operate on `XML` configuration files as a whole thanks to a configuration specification `DSL`, see [Configuration Specification Command](./ConfigurationSpecification.md);

- The ones allowing to selectively operate on individual elements of `XML` configuration files, see [Configuration Element Commands](./ConfigurationElement.md).

> **Remark** The `Dsl.Configuration` `PowerShell` module is just a façade in front of a `DSL` processing engine that is also made available as a separate `NuGet` package, see [Be.Stateless.Dsl.Configuration][nuget].

> **Tips** For the `PowerShell` newbies, you can get a list of the commands made available by this module by issuing the following `PowerShell` command:
>
> ```PowerShell
> Get-Command -Module Dsl.Configuration
> ```

## Installation

In order to be able to install the `PowerShell` module, you might have to trust the `be.stateless`'s certificate public key beforehand; see these [instructions](../../Installation.md) for details on how to proceed.

## Developer Help

Detailed developer help has been provided as `XML` comments directly embedded in source code. Though developers usually browse through this documentation while developing thanks to, for instance, JetBrains [ReSharper][resharper] quick help &mdash;<kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>F1</kbd>, an online version of this inlined help has also been provided here for greater reachability:

[![][help.cmdlets.badge]][help.cmdlets]

[![][help.badge]][help]

<!-- badges -->

[doc.install]: https://www.stateless.be/PowerShell/Module/Installation.html "PowerShell Module Installation"
[doc.main.badge]: https://img.shields.io/static/v1?label=BizTalk.Factory%20SDK&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.main]: https://www.stateless.be/ "BizTalk.Factory SDK User's Guide"
[doc.this.badge]: https://img.shields.io/static/v1?label=Dsl.Configuration&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.this]: https://www.stateless.be/PowerShell/Module/Dsl/Configuration "Dsl.Configuration PowerShell Module User's Guide"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.Dsl.Configuration&logo=github
[github]: https://github.com/icraftsoftware/Be.Stateless.Dsl.Configuration "Be.Stateless.Dsl.Configuration GitHub Repository"
[help.badge]: https://img.shields.io/static/v1?label=Be.Stateless.Dsl.Configuration&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/Dsl/Configuration/README.md "Be.Stateless.Dsl.Configuration Developer Help"
[help.cmdlets.badge]: https://img.shields.io/static/v1?label=Be.Stateless.Dsl.Configuration.Cmdlets&message=Developer%20Help&color=8CA1AF&logo=microsoftacademic
[help.cmdlets]: https://github.com/icraftsoftware/biztalk.factory.github.io/blob/master/Help/Dsl/Configuration/Cmdlets/README.md "Be.Stateless.Dsl.Configuration.Cmdlets Developer Help"
[module.badge]: https://img.shields.io/powershellgallery/v/Dsl.Configuration.svg?label=Dsl.Configuration&style=flat&logo=powershell
[module]: https://www.powershellgallery.com/packages/Dsl.Configuration "Dsl.Configuration PowerShell Module"
[module.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/Dsl.Configuration?logo=powershell
[module.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=Dsl.Configuration&protocolType=NuGet "Dsl.Configuration Preview PowerShell Module"
[nuget.badge]: https://img.shields.io/nuget/v/Be.Stateless.Dsl.Configuration.svg?label=Be.Stateless.Dsl.Configuration&style=flat&logo=nuget
[nuget]: https://www.nuget.org/packages/Be.Stateless.Dsl.Configuration "Be.Stateless.Dsl.Configuration NuGet Package"
[nuget.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/Be.Stateless.Dsl.Configuration?logo=nuget
[nuget.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=Be.Stateless.Dsl.Configuration&protocolType=NuGet "Be.Stateless.Dsl.Configuration Preview NuGet Package"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.Dsl.Configuration%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=78&branchName=master "Be.Stateless.Dsl.Configuration Continuous Integration Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.Dsl.Configuration%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=79&branchName=master "Be.Stateless.Dsl.Configuration Manual Release Build Pipeline"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.Dsl.Configuration?label=Release&logo=github
[release]: https://github.com/icraftsoftware/Be.Stateless.Dsl.Configuration/releases/latest "Be.Stateless.Dsl.Configuration GitHub Release"

<!-- links -->

[resharper]: https://www.jetbrains.com/resharper/

<!--
cSpell:ignore Cmdlets façade
-->
