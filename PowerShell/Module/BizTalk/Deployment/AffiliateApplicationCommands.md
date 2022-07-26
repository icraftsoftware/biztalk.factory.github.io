# Configuring SSO Affiliate Applications and Configuration Stores

To configure `SSO` affiliate applications, `BizTalk.Deployment` provides the following commands:

```PowerShell
Get-AffiliateApplication [[-AffiliateApplicationName] <string[]>] [<CommonParameters>]

New-AffiliateApplication [-AffiliateApplicationName] <string> [[-UserGroup] <string[]>] [<CommonParameters>]

Remove-AffiliateApplication [-AffiliateApplicationName] <string> [<CommonParameters>]
```

To configure the configuration store of an `SSO` affiliate application, `BizTalk.Deployment` provides the following commands:

```PowerShell
Get-AffiliateApplicationStore [-AffiliateApplicationName] <string[]> [-Any] [<CommonParameters>]

Update-AffiliateApplicationStore [-AffiliateApplicationName] <string> [-EnvironmentSettingsAssemblyFilePath] <string> [-TargetEnvironment] <string> [-AssemblyProbingFolderPath <string[]>] [-EnvironmentSettingOverridesTypeName <string>] [-Isolated] [<CommonParameters>]
```

> **Remark** See the native `PowerShell` help for a description of what these commands do.

> **Warning** For the `Isolated` switch to work, `PowerShell` remoting must be enabled; see how to [enable `PowerShell` remoting locally](./EnablePowerShellRemoting.md).

These commands have been primarily created to support the deployment tasks that come with the `PowerShell` module `BizTalk.Deployment` and they all rely on the `API` provided by [`Be.Stateless.BizTalk.Settings`](../../../../BizTalk/Settings/README.md). Of all of them, `Update-AffiliateApplicationStore` is the most awkward to use manually. All the others are quite intuitive and allow to easily and manually edit SSO affiliate applications and their config stores.

For instance, one can simply issue the following `PowerShell` commands to edit the properties of an affiliate application's **default** config store:

```PowerShell
$s = Get-AffiliateApplicationStore -Name 'My.App.Config.Store'
$s.Properties['Name'] = 'new-value'
$s.Save()
```

<!--
cSpell:ignore
-->
