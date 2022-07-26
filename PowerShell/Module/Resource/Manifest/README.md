# Resource.Manifest PowerShell Module

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

[![][module.badge]][module]

[![][module.preview.badge]][module.preview]

</div>
</div>

## Overview

`Resource.Manifest` is a `PowerShell` module providing commands to define resource manifests made of resource groups &mdash;i.e. resources grouped by kind. Resource manifests are declarative Microsoft BizTalk Server® deployment recipes that can be entrusted to the [`BizTalk.Deployment`][biztalk.deployment] `PowerShell` module, which will determine how a manifest's resources have to be deployed and in what order.

> **Caution** Commands provided by the `Resource.Manifest` `PowerShell` module beginning with the `New` verb have been provided with an alias that is equivalent to the noun part of the command name without the verb; e.g. `Assembly` is the alias for the `New-Assembly` command. For the `PowerShell` newbies, you can retrieve all the commands and aliases defined by the `Resource.Manifest` module via the following `PowerShell` commands:
>
> ```PowerShell
> Get-Command -Module Resource.Manifest
> Get-Alias | Where-Object Source -eq Resource.Manifest
> ```
>
> The aliases have been provided so as to make the manifests more _intuitive_ to write and understand. Only the aliases will consequently be in the subsequent documentation.

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
Assembly [-Path] <psobject[]> [[-InstallReference] <string>] [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

BamActivityModel [-Path] <psobject[]> [[-InstallReference] <string>] [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

BamIndex [-Name] <string[]> [-Activity] <string> [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

Binding  [-Path] <psobject[]> [[-AssemblyProbingFolderPath] <string[]>] [[-EnvironmentSettingOverridesTypeName] <string>] [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

EventLogSource [[-LogName] <string>] [-Name] <string[]> [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

File -Path <psobject[]> -DestinationFile <psobject[]> [-Condition <psobject>] [-PassThru] [<CommonParameters>]

File -Path <psobject[]> -DestinationFolder <psobject[]> [-Condition <psobject>] [-PassThru] [<CommonParameters>]

Installer [-Path] <psobject[]> [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

Map [-Path] <psobject[]> [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

Orchestration [-Path] <psobject[]> [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

Pipeline [-Path] <psobject[]> [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

PipelineComponent [-Path] <psobject[]> [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

ProcessDescriptor [-Path] <psobject[]> [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

Schema [-Path] <psobject[]> [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

ServiceComponent [-Path] <psobject[]> [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

SqlDatabase [-Name] <String[]> [-Server] <String> [-Path] <PSObject> [-EnlistInBizTalkBackupJob] [[-Variable] <HashTable>] [[-Condition] <PSObject>] [-PassThru] [<CommonParameters>]

SqlDeploymentScript [-Path] <psobject[]> [-Server] <string> [[-Database] <string>] [[-Variable] <HashTable>] [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

SqlUndeploymentScript [-Path] <psobject[]> [-Server] <string> [[-Database] <string>] [[-Variable] <HashTable>] [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

SsoConfigStore [-Path] <psobject[]> [[-AdministratorGroup] <string[]>] [[-UserGroup] <string[]>] [[-AssemblyProbingFolderPath] <string[]>] [[-EnvironmentSettingOverridesTypeName] <string>] [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

WindowsService [-Path] <psobject> [-Name] <string> [-Credential] <PSCredential> [[-Description] <string>] [[-DisplayName] <string>] [[-StartupType] {Automatic | AutomaticDelayedStart | Disabled | Manual}] [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

XmlConfiguration [-Path] <psobject[]> [[-Condition] <psobject>] [-PassThru] [<CommonParameters>]

XmlConfigurationAction -Path <string[]> -Delete <string> [-Condition <psobject>] [-PassThru] [<CommonParameters>]

XmlConfigurationAction -Path <string[]> -Update <string> -Attribute <HashTable> [-Condition <psobject>] [-PassThru] [<CommonParameters>]

XmlConfigurationAction -Path <string[]> -Append <string> -Name <string> [-Attribute <HashTable>] [-Condition <psobject>] [-PassThru] [<CommonParameters>]

XmlUnconfigurationAction -Path <string[]> -Delete <string> [-Condition <psobject>] [-PassThru] [<CommonParameters>]

XmlUnconfigurationAction -Path <string[]> -Update <string> -Attribute <HashTable> [-Condition <psobject>] [-PassThru] [<CommonParameters>]

XmlUnconfigurationAction -Path <string[]> -Append <string> -Name <string> [-Attribute <HashTable>] [-Condition <psobject>] [-PassThru] [<CommonParameters>]
```

> **Remark** In the previously mentioned manifests, one cannot help but notice the heavy use of the `Get-ResourceItem` command, which is a utility command that _recursively_ look for _unique_ resource files on disk underneath the manifest's current folder. Failure to locate _exactly one_ resource on disk will throw an exception.
>
> Use of this command is optional and the manifest developer can provide the resource path in any other way he sees fit

> **Remark** There exists a `New-ResourceItem` command, similarly to the `New-ResourceManifest` one, that is only meant to be used by developers who wish to extend the `Resource.Manifest` module and has not been provided with an alias, which should be a hint that this command is not meant to be used for any other purpose than extensibility ones.

## Installation

In order to be able to install the `PowerShell` module, you might have to trust the `be.stateless`'s certificate public key beforehand; see these [instructions](../../Installation.md) for details on how to proceed.

<!-- links -->

[doc.main]: https://www.stateless.be/ "BizTalk.Factory SDK"
[doc.this]: https://www.stateless.be/PowerShell/Module/Resource/Manifest/ "Resource.Manifest PowerShell Module"
[doc.install]: https://www.stateless.be/PowerShell/Module/Installation.html "PowerShell Module Installation"
[github]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.Resource.Manifest "Be.Stateless.PowerShell.Module.Resource.Manifest GitHub Repository"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.PowerShell.Module.Resource.Manifest&logo=github
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=25&branchName=master "Azure DevOps Continuous Integration Build Pipeline"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.PowerShell.Module.Resource.Manifest%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=26&branchName=master "Azure DevOps Release Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.PowerShell.Module.Resource.Manifest%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[module.preview]: https://dev.azure.com/icraftsoftware/be.stateless/_packaging?_a=package&feed=BizTalk.Factory.Preview&package=Resource.Manifest&protocolType=NuGet "Resource.Manifest PowerShell Module Preview"
[module.preview.badge]: https://badge-factory.azurewebsites.net/package/icraftsoftware/be.stateless/BizTalk.Factory.Preview/Resource.Manifest?logo=powershell
[module]: https://www.powershellgallery.com/packages/Resource.Manifest "Resource.Manifest PowerShell Module"
[module.badge]: https://img.shields.io/powershellgallery/v/Resource.Manifest.svg?label=Resource.Manifest&style=flat&logo=powershell
[release]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.Resource.Manifest/releases/latest "Be.Stateless.PowerShell.Module.Resource.Manifest GitHub Release"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.PowerShell.Module.Resource.Manifest?label=Release&logo=github

<!--  -->

[add-gac-assembly]: https://github.com/LTruijens/powershell-gac/blob/master/Add-GacAssembly.md
[biztalk.deployment]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment
[biztalk.factory.application.manifest]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Application/blob/master/src/Be.Stateless.BizTalk.Factory.Application.Deployment/Manifest.ps1
[biztalk.factory.batching.application.manifest]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Batching.Application/blob/master/src/Be.Stateless.BizTalk.Factory.Batching.Application.Deployment/Manifest.ps1
[biztalk.factory.runtime.manifest]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Runtime/blob/master/src/Be.Stateless.BizTalk.Factory.Runtime.Deployment/Manifest.ps1

<!--
cSpell:ignore BizTalkMgmtDb psobject unconfiguration unicity
-->
