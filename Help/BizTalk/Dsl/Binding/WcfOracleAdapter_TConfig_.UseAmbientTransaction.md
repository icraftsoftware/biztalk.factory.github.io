#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter&lt;TConfig&gt;](WcfOracleAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>')

## WcfOracleAdapter<TConfig>.UseAmbientTransaction Property

Specifies whether the Oracle Database adapter performs the operations using the transaction context provided by the
caller.

```csharp
public bool UseAmbientTransaction { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

The default value is `True`, which means that the adapter always performs the operations in a transaction
context, assuming that the client is providing the transactional context. If there are other resources participating
in the transaction, the connections created enlist in [System.Transactions.Transaction](https://docs.microsoft.com/en-us/dotnet/api/System.Transactions.Transaction 'System.Transactions.Transaction') and are elevated to an MSDTC
transaction.

However, there can be scenarios where you do not want the adapter to perform operations in a transactional context.
For example:
- While performing a simple SELECT operation on the Oracle database (on a send port).
- While specify a polling statement that performs a SELECT operation and does not involve any changes to the table
  either through a DELETE statement or by invoking a stored procedure (on a receive port).
Both these operations do not make any updates to the database table and hence, elevating these operations to use an
MSDTC transaction can be a performance overhead. In such scenarios, you can set the binding property to `False`
so that the Oracle Database adapter does not perform the operations in a transaction context.

Notice that not performing operations in a transactional context is advisable only for operations that do not make
changes to the database. For operations that update data in the database, we recommend setting the property to
`True` otherwise you might either experience message loss or duplicate messages depending on whether you are
performing inbound or outbound operations.