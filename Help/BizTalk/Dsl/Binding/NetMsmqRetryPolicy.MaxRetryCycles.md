#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration](Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.md 'Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration').[NetMsmqRetryPolicy](NetMsmqRetryPolicy.md 'Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.NetMsmqRetryPolicy')

## NetMsmqRetryPolicy.MaxRetryCycles Property

Gets or sets the maximum number of retry cycles to attempt delivery of messages to the receiving application.

```csharp
public virtual int MaxRetryCycles { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks
It defaults to 2.

### See Also
- [MsmqBindingBase.MaxRetryCycles](https://docs.microsoft.com/en-us/dotnet/api/system.servicemodel.msmqbindingbase.maxretrycycles#System_ServiceModel_MsmqBindingBase_MaxRetryCycles 'https://docs.microsoft.com/en-us/dotnet/api/system.servicemodel.msmqbindingbase.maxretrycycles#System_ServiceModel_MsmqBindingBase_MaxRetryCycles')