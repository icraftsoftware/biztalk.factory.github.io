#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter](WcfOracleAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter').[Inbound](WcfOracleAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound')

## WcfOracleAdapter.Inbound.InboundOperationType Property

Specifies whether you want to perform [Microsoft.Adapters.OracleDB.InboundOperation.Polling](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.OracleDB.InboundOperation.Polling 'Microsoft.Adapters.OracleDB.InboundOperation.Polling') or [Microsoft.Adapters.OracleDB.InboundOperation.Notification](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.OracleDB.InboundOperation.Notification 'Microsoft.Adapters.OracleDB.InboundOperation.Notification') inbound operation.

```csharp
public Microsoft.Adapters.OracleDB.InboundOperation InboundOperationType { get; set; }
```

#### Property Value
[Microsoft.Adapters.OracleDB.InboundOperation](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.OracleDB.InboundOperation 'Microsoft.Adapters.OracleDB.InboundOperation')

### Remarks

For more information about [Microsoft.Adapters.OracleDB.InboundOperation.Polling](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.OracleDB.InboundOperation.Polling 'Microsoft.Adapters.OracleDB.InboundOperation.Polling') see [Support
            for Receiving Polling-based Data-changed Messages in Oracle Database](https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-oracle-database/support-for-receiving-polling-based-data-changed-messages-in-oracle-database 'https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-oracle-database/support-for-receiving-polling-based-data-changed-messages-in-oracle-database') For more information about [Microsoft.Adapters.OracleDB.InboundOperation.Notification](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.OracleDB.InboundOperation.Notification 'Microsoft.Adapters.OracleDB.InboundOperation.Notification'), see [Receiving
            Oracle Database Change Notifications](https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-oracle-database/receive-oracle-database-change-notifications 'https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-oracle-database/receive-oracle-database-change-notifications').

It defaults to [Microsoft.Adapters.OracleDB.InboundOperation.Polling](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.OracleDB.InboundOperation.Polling 'Microsoft.Adapters.OracleDB.InboundOperation.Polling').