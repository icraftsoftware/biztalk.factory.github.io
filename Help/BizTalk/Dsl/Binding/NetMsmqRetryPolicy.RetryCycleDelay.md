#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration](Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.md 'Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration').[NetMsmqRetryPolicy](NetMsmqRetryPolicy.md 'Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.NetMsmqRetryPolicy')

## NetMsmqRetryPolicy.RetryCycleDelay Property

Gets or sets a value that specifies how long to wait before attempting another retry cycle when attempting to deliver
a message that could not be delivered.

```csharp
public virtual System.TimeSpan RetryCycleDelay { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks
It defaults to 10 minutes.

### See Also
- [MsmqBindingBase.RetryCycleDelay](https://docs.microsoft.com/en-us/dotnet/api/system.servicemodel.msmqbindingbase.retrycycledelay#System_ServiceModel_MsmqBindingBase_RetryCycleDelay 'https://docs.microsoft.com/en-us/dotnet/api/system.servicemodel.msmqbindingbase.retrycycledelay#System_ServiceModel_MsmqBindingBase_RetryCycleDelay')