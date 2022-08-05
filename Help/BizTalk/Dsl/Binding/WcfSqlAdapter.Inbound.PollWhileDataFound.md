#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSqlAdapter](WcfSqlAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter').[Inbound](WcfSqlAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter.Inbound')

## WcfSqlAdapter.Inbound.PollWhileDataFound Property

Controls whether the adapter should execute the Polled Data Available Statement even before the polling interval
has elapsed, if the previous execution of the polling statement returned data.

```csharp
public bool PollWhileDataFound { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')