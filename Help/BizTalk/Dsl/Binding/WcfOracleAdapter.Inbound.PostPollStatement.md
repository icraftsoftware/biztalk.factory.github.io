#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter](WcfOracleAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter').[Inbound](WcfOracleAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound')

## WcfOracleAdapter.Inbound.PostPollStatement Property

Specifies a PL/SQL block that is executed after the [PollingStatement](WcfOracleAdapter.Inbound.PollingStatement.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound.PollingStatement') and before the /POLLINGSTMT
message is sent to the consumer.

```csharp
public string PostPollStatement { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

The post-poll statement executes inside the polling transaction. Two common uses for the post-poll statement are
to:
- Update a column in the rows returned in the polling statement to indicate that they have been processed and should
  be excluded from subsequent polling queries.
- Move processed records to a different table.

If a [PostPollStatement](WcfOracleAdapter.Inbound.PostPollStatement.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound.PostPollStatement') is specified, [PollingInterval](WcfOracleAdapter.Inbound.PollingInterval.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound.PollingInterval') should be set large enough for
the PL/SQL block to complete before the interval expires.

For more information about polling, see .

It defaults to [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty'); no post-poll statement is executed.