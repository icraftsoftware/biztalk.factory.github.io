#### [Be.Stateless.Dsl.Configuration.Cmdlets](README.md 'README')
### [Be.Stateless.Dsl.Configuration.Cmdlet](Be.Stateless.Dsl.Configuration.Cmdlet.md 'Be.Stateless.Dsl.Configuration.Cmdlet')

## SetConfigurationElement Class

Set the attributes of an existing configuration element.

```csharp
public class SetConfigurationElement : Be.Stateless.Dsl.Configuration.Cmdlet.ConfigurationElementCmdlet
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.Management.Automation.Internal.InternalCommand](https://docs.microsoft.com/en-us/dotnet/api/System.Management.Automation.Internal.InternalCommand 'System.Management.Automation.Internal.InternalCommand') &#129106; [System.Management.Automation.Cmdlet](https://docs.microsoft.com/en-us/dotnet/api/System.Management.Automation.Cmdlet 'System.Management.Automation.Cmdlet') &#129106; [ConfigurationElementCmdlet](ConfigurationElementCmdlet.md 'Be.Stateless.Dsl.Configuration.Cmdlet.ConfigurationElementCmdlet') &#129106; SetConfigurationElement

### Example

```csharp
PS> Set-ConfigurationElement -TargetConfigurationFile global:machine.config -XPath "/configuration/appSettings/add[@key='setting1']" -Attributes @{ value = 'value1' }
```

| Properties | |
| :--- | :--- |
| [Action](SetConfigurationElement.Action.md 'Be.Stateless.Dsl.Configuration.Cmdlet.SetConfigurationElement.Action') | |
| [Attributes](SetConfigurationElement.Attributes.md 'Be.Stateless.Dsl.Configuration.Cmdlet.SetConfigurationElement.Attributes') | |

| Methods | |
| :--- | :--- |
| [CreateAction()](SetConfigurationElement.CreateAction().md 'Be.Stateless.Dsl.Configuration.Cmdlet.SetConfigurationElement.CreateAction()') | |
