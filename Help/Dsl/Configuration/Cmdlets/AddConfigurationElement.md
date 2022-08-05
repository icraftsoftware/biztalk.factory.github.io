#### [Be.Stateless.Dsl.Configuration.Cmdlets](README.md 'README')
### [Be.Stateless.Dsl.Configuration.Cmdlet](Be.Stateless.Dsl.Configuration.Cmdlet.md 'Be.Stateless.Dsl.Configuration.Cmdlet')

## AddConfigurationElement Class

Adds a configuration element.

```csharp
public class AddConfigurationElement : Be.Stateless.Dsl.Configuration.Cmdlet.ConfigurationElementCmdlet
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.Management.Automation.Internal.InternalCommand](https://docs.microsoft.com/en-us/dotnet/api/System.Management.Automation.Internal.InternalCommand 'System.Management.Automation.Internal.InternalCommand') &#129106; [System.Management.Automation.Cmdlet](https://docs.microsoft.com/en-us/dotnet/api/System.Management.Automation.Cmdlet 'System.Management.Automation.Cmdlet') &#129106; [ConfigurationElementCmdlet](ConfigurationElementCmdlet.md 'Be.Stateless.Dsl.Configuration.Cmdlet.ConfigurationElementCmdlet') &#129106; AddConfigurationElement

### Example

```csharp
PS> Add-ConfigurationElement -TargetConfigurationFile global:machine.config -XPath '/configuration/appSettings' -ElementName 'add' -Attributes @{ key = 'setting1'; value = 'value1' }
```

| Properties | |
| :--- | :--- |
| [Action](AddConfigurationElement.Action.md 'Be.Stateless.Dsl.Configuration.Cmdlet.AddConfigurationElement.Action') | |
| [Attributes](AddConfigurationElement.Attributes.md 'Be.Stateless.Dsl.Configuration.Cmdlet.AddConfigurationElement.Attributes') | |
| [ElementName](AddConfigurationElement.ElementName.md 'Be.Stateless.Dsl.Configuration.Cmdlet.AddConfigurationElement.ElementName') | |

| Methods | |
| :--- | :--- |
| [CreateAction()](AddConfigurationElement.CreateAction().md 'Be.Stateless.Dsl.Configuration.Cmdlet.AddConfigurationElement.CreateAction()') | |
