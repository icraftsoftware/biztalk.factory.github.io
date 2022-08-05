#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration](Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.md 'Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration').[NetMsmqRetryPolicy](NetMsmqRetryPolicy.md 'Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.NetMsmqRetryPolicy')

## NetMsmqRetryPolicy.TimeToLive Property

Gets or sets a value that specifies how long messages are valid. When this time has elapsed, the message is placed in
a dead-letter queue (if available).

```csharp
public virtual System.TimeSpan TimeToLive { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks
It defaults to 1 day.

### See Also
- [MsmqBindingBase.TimeToLive](https://docs.microsoft.com/en-us/dotnet/api/system.servicemodel.msmqbindingbase.timetolive#System_ServiceModel_MsmqBindingBase_TimeToLive 'https://docs.microsoft.com/en-us/dotnet/api/system.servicemodel.msmqbindingbase.timetolive#System_ServiceModel_MsmqBindingBase_TimeToLive')