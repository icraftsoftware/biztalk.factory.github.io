#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter](WcfOracleAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter').[Inbound](WcfOracleAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound')

## WcfOracleAdapter.Inbound.PollingStatement Property

Specifies the polling statement.

```csharp
public string PollingStatement { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

You can specify a simple SELECT statement or a stored procedure, function, or a packaged procedure or function for
polling.
- If you want to poll a table or view, you must specify a SELECT query in this binding property.
- If you want to poll using a stored procedure, function, or procedure or function within a package, you must
  specify the entire request message for the respective operation in this binding property.

The polling statement is executed only if the statement executed by the [PolledDataAvailableStatement](WcfOracleAdapter.Inbound.PolledDataAvailableStatement.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound.PolledDataAvailableStatement')
property returns some data.

The Oracle Database adapter executes the polling statement and the post-poll statement (if specified) inside of an
Oracle transaction. If you are using a SELECT statement in the [PollingStatement](WcfOracleAdapter.Inbound.PollingStatement.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound.PollingStatement') property, we
recommend that you specify a FOR UPDATE clause in your SELECT statement. This will ensure that the selected
records are locked during the transaction and that the post-poll statement can perform any required updates on the
selected records.

For more information about polling, including the use of the FOR UPDATE clause, see .