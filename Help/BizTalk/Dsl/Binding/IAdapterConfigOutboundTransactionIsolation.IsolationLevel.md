#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigOutboundTransactionIsolation](IAdapterConfigOutboundTransactionIsolation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundTransactionIsolation')

## IAdapterConfigOutboundTransactionIsolation.IsolationLevel Property

Specify the Isolation Level for the transaction.

```csharp
System.Transactions.IsolationLevel IsolationLevel { get; set; }
```

#### Property Value
[System.Transactions.IsolationLevel](https://docs.microsoft.com/en-us/dotnet/api/System.Transactions.IsolationLevel 'System.Transactions.IsolationLevel')

### Remarks
It defaults to [System.Transactions.IsolationLevel.Serializable](https://docs.microsoft.com/en-us/dotnet/api/System.Transactions.IsolationLevel.Serializable 'System.Transactions.IsolationLevel.Serializable').