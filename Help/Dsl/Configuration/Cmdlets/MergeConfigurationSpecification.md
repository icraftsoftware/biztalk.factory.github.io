#### [Be.Stateless.Dsl.Configuration.Cmdlets](README.md 'README')
### [Be.Stateless.Dsl.Configuration.Cmdlet](Be.Stateless.Dsl.Configuration.Cmdlet.md 'Be.Stateless.Dsl.Configuration.Cmdlet')

## MergeConfigurationSpecification Class

Merges specification file(s) to one ore more configuration files.

```csharp
public class MergeConfigurationSpecification : System.Management.Automation.PSCmdlet
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.Management.Automation.Internal.InternalCommand](https://docs.microsoft.com/en-us/dotnet/api/System.Management.Automation.Internal.InternalCommand 'System.Management.Automation.Internal.InternalCommand') &#129106; [System.Management.Automation.Cmdlet](https://docs.microsoft.com/en-us/dotnet/api/System.Management.Automation.Cmdlet 'System.Management.Automation.Cmdlet') &#129106; [System.Management.Automation.PSCmdlet](https://docs.microsoft.com/en-us/dotnet/api/System.Management.Automation.PSCmdlet 'System.Management.Automation.PSCmdlet') &#129106; MergeConfigurationSpecification

### Example

```csharp
PS> Merge-ConfigurationSpecification -Path ./machine.config
```

| Properties | |
| :--- | :--- |
| [ConfigurationFileResolvers](MergeConfigurationSpecification.ConfigurationFileResolvers.md 'Be.Stateless.Dsl.Configuration.Cmdlet.MergeConfigurationSpecification.ConfigurationFileResolvers') | |
| [CreateBackup](MergeConfigurationSpecification.CreateBackup.md 'Be.Stateless.Dsl.Configuration.Cmdlet.MergeConfigurationSpecification.CreateBackup') | |
| [CreateUndo](MergeConfigurationSpecification.CreateUndo.md 'Be.Stateless.Dsl.Configuration.Cmdlet.MergeConfigurationSpecification.CreateUndo') | |
| [LiteralPath](MergeConfigurationSpecification.LiteralPath.md 'Be.Stateless.Dsl.Configuration.Cmdlet.MergeConfigurationSpecification.LiteralPath') | |
| [PassThru](MergeConfigurationSpecification.PassThru.md 'Be.Stateless.Dsl.Configuration.Cmdlet.MergeConfigurationSpecification.PassThru') | |
| [Path](MergeConfigurationSpecification.Path.md 'Be.Stateless.Dsl.Configuration.Cmdlet.MergeConfigurationSpecification.Path') | |

| Methods | |
| :--- | :--- |
| [BeginProcessing()](MergeConfigurationSpecification.BeginProcessing().md 'Be.Stateless.Dsl.Configuration.Cmdlet.MergeConfigurationSpecification.BeginProcessing()') | |
| [ProcessRecord()](MergeConfigurationSpecification.ProcessRecord().md 'Be.Stateless.Dsl.Configuration.Cmdlet.MergeConfigurationSpecification.ProcessRecord()') | |
