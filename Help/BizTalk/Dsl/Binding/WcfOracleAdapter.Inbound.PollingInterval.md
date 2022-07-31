#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter](WcfOracleAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter').[Inbound](WcfOracleAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound')

## WcfOracleAdapter.Inbound.PollingInterval Property

Specifies the transacted polling interval, that is, the time interval at which the Oracle Database adapter
executes the polling statement against the Oracle database.

```csharp
public System.TimeSpan PollingInterval { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks

The polling interval is used by the adapter for the following:
- The time interval between successive polls. This interval is used to run the poll and post-poll queries. If these
  queries are executed within the specified interval, the adapter sleeps for the remaining time in the interval.
- The polling transaction timeout value. This value must be set large enough to include the polling statement
  execution time, the post-poll statement (if specified) execution time, and the time to receive the reply from the
  client application to commit the transaction.

If the client application sends a reply before the polling interval expires, the adapter commits the transaction
and waits until the polling interval is reached to execute the next poll.

If the client application returns a fault, the adapter terminates the transaction.

If the polling interval expires before the client application sends the reply, the transaction will time out. For
more information about polling, see .

The default is 500 seconds.