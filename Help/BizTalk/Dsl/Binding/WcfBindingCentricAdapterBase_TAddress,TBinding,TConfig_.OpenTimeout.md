#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfBindingCentricAdapterBase&lt;TAddress,TBinding,TConfig&gt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')

## WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.OpenTimeout Property

Gets or sets the interval of time after which the open method, invoked by a communication object, times out.

```csharp
public System.TimeSpan OpenTimeout { get; set; }
```

Implements [OpenTimeout](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts.OpenTimeout 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts.OpenTimeout')

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

#### Exceptions

[System.ArgumentOutOfRangeException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentOutOfRangeException 'System.ArgumentOutOfRangeException')  
The value is less than zero or too large.

### Remarks
The interval of time provided for a connection to open before the transport raises an exception. The default value is
1 minute.