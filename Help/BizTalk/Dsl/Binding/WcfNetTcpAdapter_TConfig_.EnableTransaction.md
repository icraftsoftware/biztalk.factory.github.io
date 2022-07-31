#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetTcpAdapter&lt;TConfig&gt;](WcfNetTcpAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter<TConfig>')

## WcfNetTcpAdapter<TConfig>.EnableTransaction Property

Specify whether a message is send under transaction scope.

```csharp
public bool EnableTransaction { get; set; }
```

Implements [EnableTransaction](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTransactions.EnableTransaction 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTransactions.EnableTransaction')

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

For outbound NetTcp adapters, it specifies whether a message is transmitted to the destination service and deleted
from the MessageBox database in a transactional context using the transaction protocol specified in the [TransactionProtocol](WcfNetTcpAdapter_TConfig_.TransactionProtocol.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter<TConfig>.TransactionProtocol') property.

For inbound NetTcp adapters, it specifies whether a message is submitted to the MessageBox database using the
transaction flowed from clients. If this property is set to `True`, the clients are required to submit messages
using the transaction protocol specified in the [TransactionProtocol](WcfNetTcpAdapter_TConfig_.TransactionProtocol.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter<TConfig>.TransactionProtocol') property. If the clients submit
messages outside the transactional scope then the receive location returns an exception back to the clients, and no
messages are suspended.

The option is available only for one-way receive locations. If the clients submit messages in a transactional context
for request-response receive locations, then an exception is returned back to the clients and no messages are
suspended.

It defaults to `False`.