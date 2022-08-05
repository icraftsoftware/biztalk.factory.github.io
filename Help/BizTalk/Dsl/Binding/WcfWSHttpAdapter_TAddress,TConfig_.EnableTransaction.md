#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWSHttpAdapter&lt;TAddress,TConfig&gt;](WcfWSHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter<TAddress,TConfig>')

## WcfWSHttpAdapter<TAddress,TConfig>.EnableTransaction Property

Specify whether a message is submitted to the MessageBox database using the transaction flowed from clients.

```csharp
public bool EnableTransaction { get; set; }
```

Implements [EnableTransaction](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTransactions.EnableTransaction 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTransactions.EnableTransaction')

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

If this property is `True`, the clients are required to submit messages using the WS-AtomicTransaction protocol.
If the clients submit messages outside the transactional scope then this receive location returns an exception back
to the clients and no messages are suspended.
            The option is available only for one-way receive locations. If the clients submit messages in a transactional context
            for request-response receive locations, then an exception is returned back to the clients and no messages are
            suspended.
            

It defaults to `False`.