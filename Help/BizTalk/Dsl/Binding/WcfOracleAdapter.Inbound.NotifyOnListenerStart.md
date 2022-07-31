#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter](WcfOracleAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter').[Inbound](WcfOracleAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound')

## WcfOracleAdapter.Inbound.NotifyOnListenerStart Property

Specifies whether the adapter sends a notification message to the adapter clients, informing that the receive
location is running, when the listener starts.

```csharp
public bool NotifyOnListenerStart { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks
It defaults is to `True`.