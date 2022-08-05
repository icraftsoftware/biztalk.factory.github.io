#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSqlAdapter](WcfSqlAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter').[Inbound](WcfSqlAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter.Inbound')

## WcfSqlAdapter.Inbound.PolledDataAvailableStatement Property

This statement is executed to determine whether data is available to be polled. Execution of this statement should
return a single result set consisting of one row and one column, the value in which should reflect the number of
rows available to be read.

```csharp
public string PolledDataAvailableStatement { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')