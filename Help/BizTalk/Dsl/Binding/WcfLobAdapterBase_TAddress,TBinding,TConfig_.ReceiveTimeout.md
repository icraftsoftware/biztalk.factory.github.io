#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfLobAdapterBase&lt;TAddress,TBinding,TConfig&gt;](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>')

## WcfLobAdapterBase<TAddress,TBinding,TConfig>.ReceiveTimeout Property

Gets or sets the interval of time after which the receive method, invoked by a communication object, times out.

```csharp
public System.TimeSpan ReceiveTimeout { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

#### Exceptions

[System.ArgumentOutOfRangeException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentOutOfRangeException 'System.ArgumentOutOfRangeException')  
The value is less than zero or too large.

### Remarks

The interval of time that a connection can remain inactive, during which no application messages are received, before
it is dropped. The default value is 10 minute.

For inbound operations such as receiving IDOCs, it is recommend to set the timeout to the maximum possible value,
which is 24.20:31:23.6470000 (24 days). When using the adapter with BizTalk Server, setting the timeout to a large
value does not impact the functionality of the adapter.