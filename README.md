# BizTalk.Factory Overview

BizTalk.Factory 2.0 is a Microsoft BizTalk Server® 2020 software development kit like many others out there, be it [BizTalk Server Pipeline Component Wizard](https://btsplcw.codeplex.com/), [BizTalk Software Factory](https://bsf.codeplex.com/) (not to be confused with BizTalk.Factory itself), Eliasen's [BizTalk Pipeline Components](https://eebiztalkpipelinecom.codeplex.com/), [BizTalk Deployment Framework](https://github.com/BTDF/DeploymentFramework), and so on.

BizTalk.Factory however is far more reaching and takes a very unique and distinctive approach: instead of being based on, or leveraging, designer surfaces or wizards, it strives to provide a code centric, or code-first, development experience. Wherever possible, BizTalk Factory will offer a C# fluent API to replace the designer surface. Note that BizTalk.Factory will not try to replace the Microsoft BizTalk Server® orchestration designer surface.

## Main Packages

BizTalk.Factory is broadly made of up of series of .NET assemblies, Microsoft BizTalk Server® applications, Microsoft SQL Server databases, and PowerShell modules. From the ground up, it consists of the following individually deployable packages:

- [BizTalk.Factory Runtime](./BizTalk/Factory/Runtime/README.md) is a Microsoft BizTalk Server® runtime made of .NET assemblies that can be deployed without any Microsoft BizTalk Server®'s footprint; it merely requires assemblies to be GAC-deployed and machine.config to be edited. Notice that since this package has no Microsoft BizTalk Server®'s footprint, it can be patched or even fully redeployed at any time without any other impact on the Microsoft BizTalk Server® Group than a small down time;

- [BizTalk.Factory Application](./BizTalk/Factory/Application/README.md) is a scaffolding  Microsoft BizTalk Server® Application, similarly to the built-in BizTalk.System Application. This application has been built as an *empty shell* consisting of a few general purpose Microsoft BizTalk Server® artifacts (e.g. context properties, pipeline components, pipelines, and schemas) that delegate the vast majority of their work to the runtime. This package consequently should almost never need to be patched or even redeployed and can therefore be relied upon and referenced by any other Microsoft BizTalk Server® applications without concern. Among the rich features this application offers, the micro-pipelines are the most valuable;











- A [BizTalk.Factory.Tracking](https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Activity.Tracking.Application) add-on application, whose [package](https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Activity.Tracking.Application/releases/latest/download/Be.Stateless.BizTalk.Factory.Activity.Tracking.Application.Deployment.zip) needs to be deployed as a full-fledged Microsoft BizTalk Server® application. This application relies on the main BizTalk.Factory application but does not need to be referenced by any other Microsoft BizTalk Server® 2020 applications, should they even rely on any of its features;

- A [BizTalk.Factory.Batching](https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Batching.Application) add-on application, whose [package](https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Batching.Application/releases/latest/download/Be.Stateless.BizTalk.Factory.Batching.Application.Deployment.zip) needs to be deployed as a full-fledged Microsoft BizTalk Server® application. This application relies on both BizTalk.Factory main and BizTalk.Factory.Tracking applications and generally needs to be referenced by any Microsoft BizTalk Server® applications that relies on any of its features;

and of the following PowerShell modules publicly available on [PowerShell Gallery](https://www.powershellgallery.com/profiles/icraftsoftware):

- [Psx](https://www.powershellgallery.com/packages/Psx) is a general scaffolding PowerShell utility module;

- [Exec](https://www.powershellgallery.com/packages/Exec) is a PowerShell utility module providing commands to work with external executables;

- [Dsl.Configuration](https://www.powershellgallery.com/packages/Dsl.Configuration) is a PowerShell utility module providing commands for general purpose XML configuration file edition;

- [Resource.Manifest](https://www.powershellgallery.com/packages/Resource.Manifest) is an extensible PowerShell utility module providing commands to define and process resource manifests that can later on be used to drive operations, in a declarative way, according to the nature of the resources to operate upon;

- [BizTalk.Administration](https://www.powershellgallery.com/packages/BizTalk.Administration) is a PowerShell utility module providing commands to administrate, configure, and explore Microsoft BizTalk Server®;

- [BizTalk.Deployment](https://www.powershellgallery.com/packages/BizTalk.Deployment) is an extensible PowerShell utility module based on a deployment framework featuring a declarative task model and providing commands to deploy full-fledged Microsoft BizTalk Server® applications. This module furthermore depends on the following third-party PowerShell Modules:
    - [Gac](https://www.powershellgallery.com/packages/Gac);
    - [InvokeBuild](https://www.powershellgallery.com/packages/InvokeBuild);
    - [SqlServer](https://www.powershellgallery.com/packages/SqlServer).

<br/>

> **Important Remark**
> To develop and even *unit* test any Microsoft BizTalk Server® artifacts (with the exception of orchestrations), none of these packages needs to be deployed as all of the required and necessary .NET assemblies to write code against are publicly available on [NuGet](https://www.nuget.org/profiles/icraftsoftware).

<br/>

## BizTalk.Factory Main Application
Components

## BizTalk.Factory.Tracking Application
Components + Claim Check + Claim Store Agent

## BizTalk.Factory.Batching Application
Components

DSL components
Config
Pipeline
Binding
Rule


## DSL Configuration PowerShell Module
Components

## BizTalk.Deployment PowerShell Module
Components


- Plain .NET assemblies
- Microsoft BizTalk Server®'s centric Domain Specific Language (DSL)
- Microsoft BizTalk Server® unit test libraries
- Microsoft BizTalk Server® applications
- Windows PowerShell modules

<!--
cSpell:ignore Eliasen, BizTalkMgmtDb
-->
