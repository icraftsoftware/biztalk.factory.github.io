# Consuming Code-First Application Bindings

We have seen that `C#` code-first bindings will be used at deployment time to generate the `XML` bindings to be imported in Microsoft BizTalk Server® for the targeted environment, see `Be.Stateless.BizTalk.Dsl.Binding` [Rationale](../../../../BizTalk/Dsl/Binding/README.md#rationale), but we have not seen how this could be achieved. The `PowerShell` module `BizTalk.Deployment` provides a variety of commands to consume these compiled assemblies containing the `C#` code-first bindings and do just that and more:

```PowerShell
Convert-ApplicationBinding [-ApplicationBindingAssemblyFilePath] <string> [-AssemblyProbingFolderPath <string[]>] [-EnvironmentSettingOverridesTypeName <string>] [-Isolated] [-OutputFilePath] <string> [-TargetEnvironment] <string> [<CommonParameters>]

Expand-ApplicationBinding [-InputFilePath] <string> [[-OutputFilePath] <string>] [-Trim] [<CommonParameters>]

Get-ApplicationHosts [-ApplicationBindingAssemblyFilePath] <string> [-AssemblyProbingFolderPath <string[]>] [-EnvironmentSettingOverridesTypeName <string>] [-Isolated] [-TargetEnvironment] <string> [<CommonParameters>]

Initialize-ApplicationState [-ApplicationBindingAssemblyFilePath] <string> [-AssemblyProbingFolderPath <string[]>] [-EnvironmentSettingOverridesTypeName <string>] [-InitializationOption {None | Orchestrations | ReceiveLocations | SendPorts | All}] [-Isolated] [-TargetEnvironment] <string> [<CommonParameters>]

Install-ApplicationFileAdapterFolders [-ApplicationBindingAssemblyFilePath] <string> [-TargetEnvironment] <string> -User <string[]> [-AssemblyProbingFolderPath <string[]>] [-EnvironmentSettingOverridesTypeName <string>] [-Isolated] [<CommonParameters>]

Test-ApplicationBinding [-ApplicationBindingAssemblyFilePath] <string> [-TargetEnvironment] <string> [-AssemblyProbingFolderPath <string[]>] [-EnvironmentSettingOverridesTypeName <string>] [-Isolated] [<CommonParameters>]

Test-ApplicationState [-ApplicationBindingAssemblyFilePath] <string> [-TargetEnvironment] <string> [-AssemblyProbingFolderPath <string[]>] [-EnvironmentSettingOverridesTypeName <string>] [-Isolated] [<CommonParameters>]

Uninstall-ApplicationFileAdapterFolders [-ApplicationBindingAssemblyFilePath] <string> [-TargetEnvironment] <string> [-AssemblyProbingFolderPath <string[]>] [-EnvironmentSettingOverridesTypeName <string>] [-Isolated] [-Recurse] [<CommonParameters>]
```

> **Remark** See the native `PowerShell` help for a description of what these commands do.

> **Warning** For the `Isolated` switch to work, `PowerShell` remoting must be enabled; see how to [enable `PowerShell` remoting locally](./EnablePowerShellRemoting.md).

These commands have been primarily created to support the deployment tasks that come with the `PowerShell` module `BizTalk.Deployment`. They are all, but the `Expand-ApplicationBinding` command, backed up by an implementation of the [`IApplicationBindingVisitor`][i-application-binding-visitor] interface, provided either directly by [`Be.Stateless.BizTalk.Dsl.Binding`](../../../../BizTalk/Dsl/Binding/README.md) assembly or by the `PowerShell` module `BizTalk.Deployment` itself, see [Consuming Code-First Bindings](../../../../BizTalk/Dsl/Binding/README.md#consuming-code-first-bindings).

- `Convert-ApplicationBinding` naturally relies on the [BindingInfoBuilder][binding-info-builder] visitor;

- `Get-ApplicationHosts` relies on the [BizTalkHostEnumerator][biztalk-host-enumerator] visitor, which also implements the `IEnumerable<string>` interface;

- `Initialize-ApplicationState` relies on the [BizTalkServiceStateInitializer][biztalk-service-state-initializer] visitor;

- `Install-ApplicationFileAdapterFolders` relies on the [FileAdapterFolderInstaller][file-adapter-folder-installer] visitor;

- `Test-ApplicationBinding` relies on the [ApplicationBindingValidator][application-binding-validator] visitor;

- `Test-ApplicationState` relies on the [BizTalkServiceStateValidator][biztalk-service-state-validator] visitor;

- `Uninstall-ApplicationFileAdapterFolders` relies on the [FileAdapterFolderUninstaller][file-adapter-folder-uninstaller] visitor.

<!-- links -->

[application-binding-validator]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Visitor/ApplicationBindingValidator.cs
[binding-info-builder]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Visitor/BindingInfoBuilder.cs
[biztalk-host-enumerator]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment/blob/master/src/Be.Stateless.BizTalk.Deployment.Cmdlets/Dsl/Binding/Visitor/BizTalkHostEnumerator.cs
[biztalk-service-state-initializer]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment/blob/master/src/Be.Stateless.BizTalk.Deployment.Cmdlets/Dsl/Binding/Visitor/BizTalkServiceStateInitializer.cs
[biztalk-service-state-validator]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment/blob/master/src/Be.Stateless.BizTalk.Deployment.Cmdlets/Dsl/Binding/Visitor/BizTalkServiceStateValidator.cs
[file-adapter-folder-installer]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment/blob/master/src/Be.Stateless.BizTalk.Deployment.Cmdlets/Dsl/Binding/Visitor/FileAdapterFolderInstaller.cs
[file-adapter-folder-uninstaller]: https://github.com/icraftsoftware/Be.Stateless.PowerShell.Module.BizTalk.Deployment/blob/master/src/Be.Stateless.BizTalk.Deployment.Cmdlets/Dsl/Binding/Visitor/FileAdapterFolderUninstaller.cs
[i-application-binding-visitor]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/IApplicationBindingVisitor.cs

<!--
cSpell:ignore
-->
