#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSqlAdapter](WcfSqlAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter').[Outbound](WcfSqlAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter.Outbound')

## WcfSqlAdapter.Outbound.BatchSize Property

The number of rows to buffer in memory before attempting an Insert, Update or Delete operation. A higher value can
improve performance, but requires more memory consumption.

```csharp
public int BatchSize { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')