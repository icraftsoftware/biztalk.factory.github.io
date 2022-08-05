#### [Be.Stateless.BizTalk.Claim.Store.Agent](README.md 'README')
### [Be.Stateless.BizTalk.Claim.Store.Configuration](Be.Stateless.BizTalk.Claim.Store.Configuration.md 'Be.Stateless.BizTalk.Claim.Store.Configuration')

## AgentConfigurationElement Class

```csharp
public sealed class AgentConfigurationElement : System.Configuration.ConfigurationElement
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.Configuration.ConfigurationElement](https://docs.microsoft.com/en-us/dotnet/api/System.Configuration.ConfigurationElement 'System.Configuration.ConfigurationElement') &#129106; AgentConfigurationElement

| Properties | |
| :--- | :--- |
| [CheckInDirectories](AgentConfigurationElement.CheckInDirectories.md 'Be.Stateless.BizTalk.Claim.Store.Configuration.AgentConfigurationElement.CheckInDirectories') | The collection of folders to collect claimed and tracked message bodies from, that is the local directories where they have been checked in. |
| [CheckOutDirectory](AgentConfigurationElement.CheckOutDirectory.md 'Be.Stateless.BizTalk.Claim.Store.Configuration.AgentConfigurationElement.CheckOutDirectory') | The directory where to drop collected claimed and tracked message bodies, that is the central directory from where they can be checked out. |
| [FileLockTimeout](AgentConfigurationElement.FileLockTimeout.md 'Be.Stateless.BizTalk.Claim.Store.Configuration.AgentConfigurationElement.FileLockTimeout') | The [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan') interval to wait before considering a lock that has been taken on a claimed or tracked message body file was not correctly released. |
| [PollingInterval](AgentConfigurationElement.PollingInterval.md 'Be.Stateless.BizTalk.Claim.Store.Configuration.AgentConfigurationElement.PollingInterval') | The [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan') interval to wait before scheduling the next collection. |
| [Properties](AgentConfigurationElement.Properties.md 'Be.Stateless.BizTalk.Claim.Store.Configuration.AgentConfigurationElement.Properties') | Gets the collection of properties. |
