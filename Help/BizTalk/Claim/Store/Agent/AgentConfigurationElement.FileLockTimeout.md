#### [Be.Stateless.BizTalk.Claim.Store.Agent](README.md 'README')
### [Be.Stateless.BizTalk.Claim.Store.Configuration](Be.Stateless.BizTalk.Claim.Store.Configuration.md 'Be.Stateless.BizTalk.Claim.Store.Configuration').[AgentConfigurationElement](AgentConfigurationElement.md 'Be.Stateless.BizTalk.Claim.Store.Configuration.AgentConfigurationElement')

## AgentConfigurationElement.FileLockTimeout Property

The [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan') interval to wait before considering a lock that has been taken on a claimed or tracked
message body file was not correctly released.

```csharp
public System.TimeSpan FileLockTimeout { get; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')