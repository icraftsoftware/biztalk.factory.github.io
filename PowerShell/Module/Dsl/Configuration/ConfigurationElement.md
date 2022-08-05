# Configuration Element Commands

> **Tip** For the `PowerShell` newbies, you can then get the signature of all the configuration element commands via the following `PowerShell` command:
>
> ```PowerShell
> Get-Command -Noun ConfigurationElement | Get-Help
> ```

The `Dsl.Configuration` `PowerShell` module provides three commands to selectively edit individual element in `XML` configuration files:

```PowerShell
Add-ConfigurationElement -TargetConfigurationFile <string[]> -XPath <string> -ElementName <string> [-Attribute <HashTable>] [-ConfigurationFileResolver <IConfigurationFileResolverStrategy[]>] [-WhatIf] [-Confirm] [<CommonParameters>]

Remove-ConfigurationElement -TargetConfigurationFile <string[]> -XPath <string> [-ConfigurationFileResolver <IConfigurationFileResolverStrategy[]>] [-WhatIf] [-Confirm] [<CommonParameters>]

Set-ConfigurationElement -TargetConfigurationFile <string[]> -XPath <string> [-Attribute <HashTable>] [-ConfigurationFileResolver <IConfigurationFileResolverStrategy[]>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

Where

- `TargetConfigurationFile` is a list of target `XML` configuration file monikers, see [Configuration File Monikers and Resolvers](./ConfigurationSpecification.md#configuration-file-monikers-and-resolvers);

- `XPath` is either the location of the element to remove or set, or the location of the parent of the element to add;

- `ElementName` is the name of the element to add;

- `Attribute` is the attributes and their values to either add to or set for the targeted element;

- `ConfigurationFileResolver` is an ordered list of object instances of classes implementing the [IConfigurationFileResolverStrategy][i-configuration-file-resolver-strategy] interface that will participate in the resolution of target configuration file monikers, see [Configuration File Monikers and Resolvers](./ConfigurationSpecification.md#configuration-file-monikers-and-resolvers).

The following excerpt provides a few usage samples of these commands:

```PowerShell
Add-ConfigurationElement -TargetConfigurationFile global:clr4:machine.config `
  -XPath /configuration/appSettings `
  -ElementName add `
  -Attribute @{ key = 'setting' ; value = 'value' }

Remove-ConfigurationElement -TargetConfigurationFile global:biztalk.config `
   -XPath /configuration/element

Set-ConfigurationElement -TargetConfigurationFile global:clr4:32bits:machine.config `
   -XPath /configuration/element `
   -Attribute @{ '{urn:custom:namespace}attribute' = 'value' }
```

> **Caution** These commands are not idempotent as are [Configuration Specification](./ConfigurationSpecification.md#configuration-specification-idempotence), that is to say that a command that completed successfully would fail if being executed again.

> **Remark** Contrary to the [Configuration Specification](ConfigurationSpecification.md) command, these commands will not perform any backup of the edited `XML` configuration files or create any inverse scripts capable of undoing all the changes that have actually been made.

<!-- links -->

[i-configuration-file-resolver-strategy]: https://github.com/icraftsoftware/Be.Stateless.Dsl.Configuration/blob/master/src/Be.Stateless.Dsl.Configuration/Dsl/Configuration/Resolver/IConfigurationFileResolverStrategy.cs

<!--
cSpell:ignore biztalk idempotence
-->
