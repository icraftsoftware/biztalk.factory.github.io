# Installing and Uninstalling Microsoft BizTalk Server® Applications

Recall that `BizTalk.Factory` is made of a series of [Runtime Packages](../../../../README.md#runtime-packages). These packages can be categorized according to whether their deployment has a Microsoft BizTalk Server® `BizTalkMgmtDb` footprint or not. Clearly [BizTalk.Factory Runtime](./BizTalk/Factory/Runtime/README.md) has none, while all the others do. The install commands plainly reflect this dichotomy: there is a pair of commands to install and uninstall `BizTalk Libraries` &mdash;thus, without `BizTalkMgmtDb` footprint:

```PowerShell
Install-BizTalkLibrary -Manifest <Hashtable[]> -TargetEnvironment <String> [-Task <ScriptBlock[]>] [-ExcludeResourceGroup <String[]>] [-ExcludeTask <String[]>] [-Isolated] [-SkipSharedResources] [-SkipUninstall] [<CommonParameters>]

Uninstall-BizTalkLibrary -Manifest <Hashtable[]> -TargetEnvironment <String> [-Task <ScriptBlock[]>] [-ExcludeResourceGroup <String[]>] [-ExcludeTask <String[]>] [-Isolated] [-SkipSharedResources] [<CommonParameters>]
```

And there is another pair of commands to install and uninstall full-fledged `BizTalk Applications` &mdash;thus, with a `BizTalkMgmtDb` footprint:

```PowerShell
Install-BizTalkApplication -Manifest <Hashtable[]> -TargetEnvironment <String> [-Task <ScriptBlock[]>] [-ExcludeResourceGroup <String[]>] [-ExcludeTask <String[]>] [-FileUser <String[]>] [-InitializationOption {None | Orchestrations | ReceiveLocations | SendPorts | All}] [-Isolated] [-SkipFileAdapterFolders] [-SkipHostInstanceRestart] [-SkipSharedResources] [-SkipUninstall] [-TerminateServiceInstances] [<CommonParameters>]

Uninstall-BizTalkApplication -Manifest <Hashtable[]> -TargetEnvironment <String> [-Task <ScriptBlock[]>] [-ExcludeResourceGroup <String[]>] [-ExcludeTask <String[]>] [-Isolated] [-SkipFileAdapterFolders] [-SkipHostInstanceRestart] [-SkipSharedResources] [-TerminateServiceInstances] [<CommonParameters>]
```

> **Remark** Each command is available in two forms, either one accepting a manifest object instance or another accepting a path to the manifest file. For simplicity's sake, only the one accepting the manifest object instance has been illustrated.

> **Remark** The help for these commands is not directly available as these commands are not actual commands per se, but aliases pointing to script files. To get the help for these scripts, one has to issue the following commands:
>
> ```PowerShell
> Import-Module -Name BizTalk.Deployment
> Get-Help -Name (Get-Alias -Name Install-BizTalkApplication).Definition -Detailed
> ```

> **Warning** For the `Isolated` switch to work, `PowerShell` remoting must be enabled; see how to [enable `PowerShell` remoting locally](./EnablePowerShellRemoting.md).

<!--
cSpell:ignore BizTalkMgmtDb Hashtable
-->
