#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter](WcfOracleAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter').[Inbound](WcfOracleAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound')

## WcfOracleAdapter.Inbound.PolledDataAvailableStatement Property

Specifies the SELECT statement executed to determine whether any data is available for polling.

```csharp
public string PolledDataAvailableStatement { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

This specified statement should return a single result set consisting of one row and one column, the value in
which should reflect the number of rows available to be read.

The default value of this binding property is set to: `SELECT 1 FROM DUAL`, which implies that the adapter
will continue polling irrespectively of whether the table being polled has data or not.

You must not specify stored procedures for this binding property. Also, this statement must not modify the
underlying Oracle database.