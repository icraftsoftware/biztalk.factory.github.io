# Resource.Manifest PowerShell Module

[![][github.badge]][github]

##### Build Pipelines

[![][pipeline.mr.badge]][pipeline.mr]

[![][pipeline.ci.badge]][pipeline.ci]

##### Latest Release

[![][module.badge]][module]

[![][release.badge]][release]

##### Release Preview

[![][module.preview.badge]][module.preview]

## Overview

`Resource.Manifest` is a `PowerShell` module providing commands to define resource manifests made of resource groups &mdash;i.e. resources grouped by kind. Resource manifests are declarative Microsoft BizTalk Server® deployment recipes that can be entrusted to the [`BizTalk.Deployment`][biztalk.deployment] `PowerShell` module, which will take care of the actual deployment.

> **Tips** Commands provided by the `Resource.Manifest` `PowerShell` module beginning with the `New` verb have been provided with an alias that is equivalent to the noun part of the command name without the verb; e.g. `Assembly` is the alias for the `New-Assembly` command. For the `PowerShell` newbies, you can retrieve all the commands and aliases defined by the `Resource.Manifest` module via the following `PowerShell` commands:
>
> ```PowerShell
> Get-Command -Module Resource.Manifest
> Get-Alias | Where-Object Source -eq Resource.Manifest
> ```
>
> The aliases have been provided so as to make the manifests more _intuitive_ to write and understand. Only the aliases will consequently be used in the subsequent documentation.

## Resource Manifests

There are two commands that allows to create resource manifests:

```PowerShell
LibraryManifest [-Name] <string> [[-Description] <string>] [-Build] <ScriptBlock> [<CommonParameters>]

ApplicationManifest [-Name] <string> [[-Description] <string>] [[-Reference] <string[]>] [[-WeakReference] <string[]>] [-Build] <ScriptBlock> [<CommonParameters>]
```

`LibraryManifest` is a command used to define deployment manifest for Microsoft BizTalk Server® packages that have no `BizTalkMgmtDb` footprint, in other words, packages that do not contain Microsoft BizTalk Server® artifacts such as orchestrations, pipelines, maps, schemas, bindings, and so on; see for instance the `BizTalk.Factory` runtime [manifest][biztalk.factory.runtime.manifest].

`ApplicationManifest` is a command used to define deployment manifest for Microsoft BizTalk Server® packages that do have a `BizTalkMgmtDb` footprint, in other words, packages that contain Microsoft BizTalk Server® artifacts such as orchestrations, pipelines, maps, schemas, bindings, and so on; see for instance the `BizTalk.Factory` application [manifest][biztalk.factory.application.manifest] or the `BizTalk.Factory.Batching` application [manifest][biztalk.factory.batching.application.manifest].

As illustrated by the previously mentioned manifests, the `Build` parameter accepts a script block that actually defines the various resources, or resource groups, that are composing the manifest.

The `WeakReference` parameter accepts a list of names of Microsoft BizTalk Server® applications that this application requires at runtime to operate correctly. This parameter comes with no `BizTalkMgmtDb` footprint and will merely check at deployment time that the listed weakly referenced applications are present.

The `Reference` parameter accepts a list of names of Microsoft BizTalk Server® applications that this application must refer to in order for its artifacts to be successfully deployed, for instance because one of its own resources uses a pipeline or a schema that is deployed by one the applications it refers to. By opposition to the `WeakReference` parameter, this _strong_ `Reference` parameter comes with a `BizTalkMgmtDb` footprint.

> **Remark** If you run the following `PowerShell` command:
>
> ```PowerShell
> Get-Command -Module Resource.Manifest -Noun *Manifest
> ```
>
> you will notice that there actually is a third command that allows to create resource manifest:
>
> ```PowerShell
> New-ResourceManifest [-Type] <string> [-Name] <string> [[-Description] <string>] [[-ItemUnicityScope] {Manifest | Resource | None}] [-Build] <ScriptBlock> [[-UnboundArguments] <Object[]>] [<CommonParameters>]
> ```
>
> `New-ResourceManifest` however is only meant to be used by developers who wish to extend the `Resource.Manifest` module and has not been provided with an alias, which should be a hint that this command is not meant to be used for any other purpose than extensibility ones.

## Resource Groups

`Resource.Manifest` supports the following resources, where each resource is just a parameterized description of what needs to deployed. The parameters of a resource command matches the parameters that its actual deployment command defines; for instance to deploy an assembly to the `GAC` the [`Add-GacAssembly`][add-gac-assembly] command mainly needs two parameters, a `Path` and an `InstallReference`, that the `Assembly` resource defining command supports as well.

```PowerShell
Assembly [-Path] <PSObject[]> [[-InstallReference] <string>] [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

BamActivityModel [-Path] <PSObject[]> [[-InstallReference] <string>] [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

BamIndex [-Name] <string[]> [-Activity] <string> [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

Binding  [-Path] <PSObject[]> [[-AssemblyProbingFolderPath] <string[]>] [[-EnvironmentSettingOverridesTypeName] <string>] [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

EventLogSource [[-LogName] <string>] [-Name] <string[]> [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

File -Path <PSObject[]> -DestinationFile <PSObject[]> [-Condition <PSObject>] [-PassThru] [<CommonParameters>]

File -Path <PSObject[]> -DestinationFolder <PSObject[]> [-Condition <PSObject>] [-PassThru] [<CommonParameters>]

Installer [-Path] <PSObject[]> [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

Map [-Path] <PSObject[]> [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

Orchestration [-Path] <PSObject[]> [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

Pipeline [-Path] <PSObject[]> [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

PipelineComponent [-Path] <PSObject[]> [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

ProcessDescriptor [-Path] <PSObject[]> [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

Schema [-Path] <PSObject[]> [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

ServiceComponent [-Path] <PSObject[]> [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

SqlDatabase [-Name] <String[]> [-Server] <String> [-Path] <PSObject> [-EnlistInBizTalkBackupJob] [[-Variable] <HashTable>] [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

SqlDeploymentScript [-Path] <PSObject[]> [-Server] <string> [[-Database] <string>] [[-Variable] <HashTable>] [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

SqlUndeploymentScript [-Path] <PSObject[]> [-Server] <string> [[-Database] <string>] [[-Variable] <HashTable>] [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

SsoConfigStore [-Path] <PSObject[]> [[-AdministratorGroup] <string[]>] [[-UserGroup] <string[]>] [[-AssemblyProbingFolderPath] <string[]>] [[-EnvironmentSettingOverridesTypeName] <string>] [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

WindowsService [-Path] <PSObject> [-Name] <string> [-Credential] <PSCredential> [[-Description] <string>] [[-DisplayName] <string>] [[-StartupType] {Automatic | AutomaticDelayedStart | Disabled | Manual}] [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

XmlConfiguration [-Path] <PSObject[]> [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

XmlConfigurationAction -Path <string[]> -Delete <string> [-Condition <PSObject>] [-PassThru] [<CommonParameters>]

XmlConfigurationAction -Path <string[]> -Update <string> -Attribute <HashTable> [-Condition <PSObject>] [-PassThru] [<CommonParameters>]

XmlConfigurationAction -Path <string[]> -Append <string> -Name <string> [-Attribute <HashTable>] [-Condition <PSObject>] [-PassThru] [<CommonParameters>]

XmlUnconfigurationAction -Path <string[]> -Delete <string> [-Condition <PSObject>] [-PassThru] [<CommonParameters>]

XmlUnconfigurationAction -Path <string[]> -Update <string> -Attribute <HashTable> [-Condition <PSObject>] [-PassThru] [<CommonParameters>]

XmlUnconfigurationAction -Path <string[]> -Append <string> -Name <string> [-Attribute <HashTable>] [-Condition <PSObject>] [-PassThru] [<CommonParameters>]
```

> **Remark** In the previously mentioned manifests, one cannot help but notice the heavy use of the `Get-ResourceItem` command, which is a utility command that _recursively_ look for _unique_ resource files on disk underneath the manifest's current folder. Failure to locate _exactly one_ resource on disk will throw an exception.
>
> Use of this command is optional and the manifest developer can provide the resource path in any other way he sees fit

> **Remark** There exists a `New-ResourceItem` command, similarly to the `New-ResourceManifest` one, that is only meant to be used by developers who wish to extend the `Resource.Manifest` module and has not been provided with an alias, which should be a hint that this command is not meant to be used for any other purpose than extensibility ones.

## Installation

In order to be able to install the `PowerShell` module, you might have to trust the `be.stateless`'s certificate public key beforehand; see these [instructions](../../Installation.md) for details on how to proceed.

<!-- badges -->

[doc.install]: https://www.stateless.be/PowerShell/Module/Installation.html "PowerShell Module Installation"
[doc.main.badge]: https://img.shields.io/static/v1?label=BizTalk.Factory%20SDK&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.main]: https://www.stateless.be/ "BizTalk.Factory SDK User's Guide"
[doc.this.badge]: https://img.shields.io/static/v1?label=Resource.Manifest&message=User's%20Guide&color=8CA1AF&logo=readthedocs
[doc.this]: https://www.stateless.be/PowerShell/Module/Resource/Manifest "Resource.Manifest PowerShell Module User's Guide"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.PowerShell.Module.Resource.Manifest&logo=github
[github]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.Resource.Manifest "Be.Stateless.PowerShell.Module.Resource.Manifest GitHub Repository"
[module.badge]: https://img.shields.io/powershellgallery/v/Resource.Manifest.svg?label=Resource.Manifest&style=flat&logo=powershell
[module]: https://www.powershellgallery.com/packages/Resource.Manifest "Resource.Manifest PowerShell Module"
[module.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/Resource.Manifest?logo=powershell
[module.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=Resource.Manifest&protocolType=NuGet "Resource.Manifest PowerShell Module Preview"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.PowerShell.Module.Resource.Manifest%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=25&branchName=master "Be.Stateless.PowerShell.Module.Resource.Manifest Continuous Integration Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.PowerShell.Module.Resource.Manifest%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=26&branchName=master "Be.Stateless.PowerShell.Module.Resource.Manifest Manual Release Build Pipeline"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.PowerShell.Module.Resource.Manifest?label=Release&logo=github
[release]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.Resource.Manifest/releases/latest "Be.Stateless.PowerShell.Module.Resource.Manifest GitHub Release"

<!-- links -->

[add-gac-assembly]: https://github.com/LTruijens/powershell-gac/blob/master/Add-GacAssembly.md
[biztalk.deployment]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment
[biztalk.factory.application.manifest]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Application/blob/master/src/Be.Stateless.BizTalk.Factory.Application.Deployment/Manifest.ps1
[biztalk.factory.batching.application.manifest]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Batching.Application/blob/master/src/Be.Stateless.BizTalk.Factory.Batching.Application.Deployment/Manifest.ps1
[biztalk.factory.runtime.manifest]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Runtime/blob/master/src/Be.Stateless.BizTalk.Factory.Runtime.Deployment/Manifest.ps1

<!--
cSpell:ignore BizTalkMgmtDb unconfiguration unicity
-->
