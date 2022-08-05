#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter&lt;TConfig&gt;](WcfNetMsmqAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>')

## WcfNetMsmqAdapter<TConfig>.EnableTransaction Property

Specify whether the message queue is transactional or non-transactional.

```csharp
public bool EnableTransaction { get; set; }
```

Implements [EnableTransaction](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTransactions.EnableTransaction 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTransactions.EnableTransaction')

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

If this property is selected, each message is delivered only once, and the sender is notified of delivery failures.
To send messages through transactional send ports, both the `durable` and `exactlyOnce` binding elements of
the client must be set to `True`. If this property is cleared, messages are transferred without delivery
assurance.
            If you use a transactional queue under this receive location, this property must be selected.
            

It defaults to `False`.