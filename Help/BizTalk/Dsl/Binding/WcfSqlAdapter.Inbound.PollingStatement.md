#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSqlAdapter](WcfSqlAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter').[Inbound](WcfSqlAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter.Inbound')

## WcfSqlAdapter.Inbound.PollingStatement Property

The SQL statement used to retrieve data from SQL, and optionally update the database. This statement will be
executed within a transaction. In BizTalk Server, this same transaction will be used to insert the message into
the Message Box.

```csharp
public string PollingStatement { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')