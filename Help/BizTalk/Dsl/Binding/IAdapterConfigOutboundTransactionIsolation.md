#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## IAdapterConfigOutboundTransactionIsolation Interface

```csharp
public interface IAdapterConfigOutboundTransactionIsolation
```

Derived  
&#8627; [Outbound&lt;TBinding&gt;](WcfCustomAdapter.Outbound_TBinding_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Outbound<TBinding>')  
&#8627; [Outbound](WcfOracleAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Outbound')  
&#8627; [Outbound](WcfSapAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound')  
&#8627; [Outbound](WcfSqlAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter.Outbound')

### See Also
- [WCF-Custom Transport Properties Dialog Box, Send, Messages Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-custom-transport-properties-dialog-box-send-messages-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-custom-transport-properties-dialog-box-send-messages-tab')

| Properties | |
| :--- | :--- |
| [EnableTransaction](IAdapterConfigOutboundTransactionIsolation.EnableTransaction.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundTransactionIsolation.EnableTransaction') | Specify whether a message is send under [System.Transactions.Transaction](https://docs.microsoft.com/en-us/dotnet/api/System.Transactions.Transaction 'System.Transactions.Transaction') scope. |
| [IsolationLevel](IAdapterConfigOutboundTransactionIsolation.IsolationLevel.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundTransactionIsolation.IsolationLevel') | Specify the Isolation Level for the transaction. |
