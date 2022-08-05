#### [Be.Stateless.Dsl.Configuration.Cmdlets](README.md 'README')
### [Be.Stateless.Dsl.Configuration.Cmdlet](Be.Stateless.Dsl.Configuration.Cmdlet.md 'Be.Stateless.Dsl.Configuration.Cmdlet')

## RemoveConfigurationElement Class

Removes an existing configuration element.

```csharp
public class RemoveConfigurationElement : Be.Stateless.Dsl.Configuration.Cmdlet.ConfigurationElementCmdlet
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.Management.Automation.Internal.InternalCommand](https://docs.microsoft.com/en-us/dotnet/api/System.Management.Automation.Internal.InternalCommand 'System.Management.Automation.Internal.InternalCommand') &#129106; [System.Management.Automation.Cmdlet](https://docs.microsoft.com/en-us/dotnet/api/System.Management.Automation.Cmdlet 'System.Management.Automation.Cmdlet') &#129106; [ConfigurationElementCmdlet](ConfigurationElementCmdlet.md 'Be.Stateless.Dsl.Configuration.Cmdlet.ConfigurationElementCmdlet') &#129106; RemoveConfigurationElement

### Example

```csharp
PS> Remove-ConfigurationElement -TargetConfigurationFile global:machine.config -XPath "/configuration/appSettings/add[@key='setting1']"
```

| Properties | |
| :--- | :--- |
| [Action](RemoveConfigurationElement.Action.md 'Be.Stateless.Dsl.Configuration.Cmdlet.RemoveConfigurationElement.Action') | |

| Methods | |
| :--- | :--- |
| [CreateAction()](RemoveConfigurationElement.CreateAction().md 'Be.Stateless.Dsl.Configuration.Cmdlet.RemoveConfigurationElement.CreateAction()') | |
