# Deployment Tasks

`BizTalk.Deployment` is an extensible `PowerShell` utility module providing a Microsoft BizTalk Server® deployment engine featuring a declarative resource-driven task model. Its resource-driven nature comes from the `PowerShell` [`Resource.Manifest`](../../Resource/Manifest/README.md) module, thanks to which a deployment package developer can write manifests declaring all the various resources that need to be deployed; see for instance the `BizTalk.Factory Runtime`'s [library manifest][biztalk-factory-runtime-manifest] or `BizTalk.Factory Application`'s [application manifest][biztalk-factory-application-manifest]. As illustrated, a manifest is just a bunch of resources, declared in no particular order, that need to be installed during the deployment of the package to which it belongs and that it describes.

To support the deployment of these resources, the `PowerShell` `BizTalk.Deployment` module provides three categories of tasks:

- _worker_ tasks, that is the tasks that carry on the actual un/deployment of resources. For each type of resources that one can declare in a manifest corresponds a series of these worker tasks, which, by convention, are named after the pluralized form of the resource. For instance, the `Assembly` resource is matched by the pair of `Deploy-Assemblies` and `Undeploy-Assemblies` deployment tasks, the `SsoConfigStore` resource is matched by the series of `Add-SsoConfigStores`, `Update-SsoConfigStores`, and `Remove-SsoConfigStores` deployment tasks, and so on...

- _extensibility_ tasks, that is the empty tasks that are meant to be overridden. These tasks are named by conventions with the `Enter-` or `Exit-` prefix. `BizTalk.Deployment` provides the following extensibility hooks:

  - `Enter-BtsDeployment` and `Exit-BtsDeployment` that provides injection hooks for tasks that need to run before or after the deployment of the various Microsoft BizTalk Server® artifacts;
  - `Enter-BtsUndeployment` and `Exit-BtsUndeployment` that provides injection hooks for tasks that need to run before or after the undeployment of the various Microsoft BizTalk Server® artifacts;
  - `Enter-DatabaseDeployment` and `Exit-DatabaseDeployment` that provides injection hooks for tasks that need to run before or after the deployment of the Microsoft SQL Server® objects;
  - `Enter-DatabaseUndeployment` and `Exit-DatabaseUndeployment` that provides injection hooks for tasks that need to run before or after the undeployment of the Microsoft SQL Server® objects.

- _organizational_ tasks, that is the tasks that tie all the previous tasks together &mdash;see [Tasks may have relations][task-relations]&mdash; in order to achieve the deployment of Microsoft BizTalk Server® deployment manifests. The tasks defined in the [Tasks.ps1][main.tasks] are all organizational ones.

> **Remark** Worker tasks are tasks that define only a body surrounded by curly braces. Organizational tasks are tasks that define only relations to other tasks. Extensibility tasks are tasks that are only declared without defining either a body or relations. See `Invoke-Build`'s [wiki][invoke-build-wiki] for a comprehensive documentation on tasks.

## Writing Custom Tasks

Once you are familiar with the [`Invoke-Build`][invoke-build-wiki] `PowerShell` module, writing custom extension tasks for `BizTalk.Deployment` is quite easy &mdash;have a look at `BizTalk.Deployment` sources for examples of writing custom [tasks][tasks] of the various categories listed above.

On top of [`Invoke-Build`][invoke-build], `BizTalk.Deployment` comes however with concepts of its own that you need to understand in order to be able to write custom tasks. There a couple of predefined variables, `$Manifest` and `$Resources`, that are automatically set and made available to the developer of custom tasks.

- `$Manifest` is a variable that points to the actual manifest instance object that is driving the deployment and is typically use to determine specifics about it and act accordingly. For instance, only inject the Microsoft BizTalk Server® deployment tasks when it is a an application manifest, as illustrated by this [line][main.tasks.for.app.manifest] of the main organizational [tasks][main.tasks];

- `$Resources` is a variable that is automatically set for each task that is about to be executed to point to the actual resource group &mdash;i.e. all the resources of the same type belonging to the manifest object instance driving the deployment&mdash; that the task is meant to work with. This can be automatically done thanks to the convention we are following, where the noun part of the task name &mdash;e.g. `Assemblies` in `Deploy-Assemblies`&mdash; matches the pluralized form of the name of the resources found in the manifest object instance &mdash;e.g. `Assembly`.

  There are however tasks that do not follow this convention, e.g. the [tasks][tasks.file.adapter.folders] that deploys the folders declared by the file adapter-based Microsoft BizTalk Server® artifacts whose configuration has been written with `BizTalk.Factory` code-first [`Binding DSL`](../../../../BizTalk/Dsl/Binding/README.md), see [Consuming Code-First Application Bindings](ApplicationBindingCommands.md). In this case, the task developer can explicitly retrieve the resource group of his choice by calling the `PowerShell` function [`Get-ResourceGroup`][get-resource-group] and passing the name of the resource group to retrieve. The developer can and should also pass a pseudo resource name that can ultimately be used by the `ExcludeResourceGroup` parameter of the installation commands &mdash;see [Installing and Uninstalling Microsoft BizTalk Server® Applications](./InstallationCommands.md)&mdash; to filter out this resource group at deployment time.

Once the custom extension tasks have been developed, you can simply pass them to `BizTalk.Deployment` through the `Task` parameter of the installation commands &mdash;see [Installing and Uninstalling Microsoft BizTalk Server® Applications](./InstallationCommands.md). Here is a quick sample that summarizes all the necessary steps that would be necessary should one want to deploy Microsoft Windows® `MSMQ` queues together with Microsoft BizTalk Server® artifacts.

1. Let us imagine that we already written a custom resource extension, `MsmqQueue`, for the [`Resource.Manifest`](../../Resource/Manifest/README.md) `PowerShell` module. We then need to override the extension tasks to inject our custom tasks as follows:

   ```PowerShell
   task Enter-BtsDeployment `
      Deploy-MsmqQueues

   task Exit-BtsUndeployment `
      Undeploy-MsmqQueues

   # Synopsis: Deploy MSMQ queues
   task Deploy-MsmqQueues {
      $Resources | ForEach-Object -Process {
         Write-Build DarkGreen $_.Name
         New-MsmqQueue -Name $_.Name -QueueType $_.Type -Transactional | Out-Null
      }
   }

   # Synopsis: Undeploy MSMQ queues
   task Undeploy-MsmqQueues {
      $Resources | ForEach-Object -Process {
         Write-Build DarkGreen $_.Name
         Get-MsmqQueue -Name $_.Name -QueueType $_.Type | Remove-MsmqQueue
      }
   }
   ```

2. Let us imagine that we pack these custom tasks in a `PowerShell` module and define an alias, `My.Deployment.Tasks`, that points to the file containing these task definitions, similarly to what `BizTalk.Deployment` does with the [`BizTalk.Deployment.Tasks`][biztalk.deployment.tasks.alias] alias.

3. To use these custom tasks, one simply has to pass them via the `Task` parameter of the installation commands as follows &mdash;notice the tasks are dot sourced through a script block argument:

   ```PowerShell
   Install-BizTalkApplication -Manifest $manifest `
      -TargetEnvironment PRD `
      -Task { . My.Deployment.Tasks }
   ```

   Provided of course that the `$manifest` instance declares `MsmqQueue` resources, these will be automatically deployed alongside the Microsoft BizTalk Server® application.

<!-- links -->

[biztalk-factory-application-manifest]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Application/blob/master/src/Be.Stateless.BizTalk.Factory.Application.Deployment/Manifest.ps1
[biztalk-factory-runtime-manifest]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Runtime/blob/master/src/Be.Stateless.BizTalk.Factory.Runtime.Deployment/Manifest.ps1
[biztalk.deployment.tasks.alias]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment/blob/master/src/BizTalk.Deployment/BizTalk.Deployment.psm1#L32
[get-resource-group]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment/blob/master/src/BizTalk.Deployment/Commands/ResourceGroup/ResourceGroup.ps1#L21
[invoke-build-wiki]: https://github.com/nightroman/Invoke-Build/wiki
[invoke-build]: https://github.com/nightroman/Invoke-Build
[main.tasks.for.app.manifest]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment/blob/master/src/BizTalk.Deployment/Tasks/Tasks.ps1#L73
[main.tasks]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment/blob/master/src/BizTalk.Deployment/Tasks/Tasks.ps1
[task-relations]: https://github.com/nightroman/Invoke-Build/wiki/Concepts#tasks-may-have-relations
[tasks.file.adapter.folders]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment/blob/master/src/BizTalk.Deployment/Tasks/Tasks.BtsFileAdapterFolders.ps1#L23
[tasks]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment/tree/master/src/BizTalk.Deployment/Tasks

<!--
cSpell:ignore MSMQ
-->
