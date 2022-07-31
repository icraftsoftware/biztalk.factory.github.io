#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter](WcfOracleAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter').[Inbound](WcfOracleAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound')

## WcfOracleAdapter.Inbound.PollWhileDataFound Property

Specifies whether the Oracle Database adapter ignores the polling interval and continuously polls the Oracle
database, if data is available in the table being polled. If no data is available in the table, the adapter
reverts to execute the SQL statement at the specified polling interval.

```csharp
public bool PollWhileDataFound { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

Consider a scenario where the polling interval is set to 60 seconds, and the statement specified for [PolledDataAvailableStatement](WcfOracleAdapter.Inbound.PolledDataAvailableStatement.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound.PolledDataAvailableStatement') returns that data is available for polling. The adapter then executes the
statement specified for the [PollingStatement](WcfOracleAdapter.Inbound.PollingStatement.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound.PollingStatement') property. Assuming that the adapter takes just 10
seconds to execute the statement, it will now have to wait for 50 seconds before executing the [PolledDataAvailableStatement](WcfOracleAdapter.Inbound.PolledDataAvailableStatement.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound.PolledDataAvailableStatement') again, and then subsequently execute the [PollingStatement](WcfOracleAdapter.Inbound.PollingStatement.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound.PollingStatement').
Instead, to optimize the performance you can set the [PollWhileDataFound](WcfOracleAdapter.Inbound.PollWhileDataFound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound.PollWhileDataFound') property to `True` so
that the adapter can start executing the next polling cycle as soon as the previous polling cycle ends.

This property is applicable both for polling on tables and views and polling using stored procedures, functions,
or packaged procedures or functions.

It defaults to `False`.