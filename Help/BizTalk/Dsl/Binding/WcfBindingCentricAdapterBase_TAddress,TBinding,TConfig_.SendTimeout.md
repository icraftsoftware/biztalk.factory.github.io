#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfBindingCentricAdapterBase&lt;TAddress,TBinding,TConfig&gt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')

## WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.SendTimeout Property

Gets or sets the interval of time after which the send method, invoked by a communication object, times out.

```csharp
public System.TimeSpan SendTimeout { get; set; }
```

Implements [SendTimeout](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts.SendTimeout 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts.SendTimeout')

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

#### Exceptions

[System.ArgumentOutOfRangeException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentOutOfRangeException 'System.ArgumentOutOfRangeException')  
The value is less than zero or too large.

### Remarks
The interval of time provided for a write operation to complete before the transport raises an exception. The default
value is 1 minute.