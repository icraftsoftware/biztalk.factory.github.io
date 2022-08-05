#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSqlAdapter&lt;TConfig&gt;](WcfSqlAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter<TConfig>')

## WcfSqlAdapter<TConfig>.UseAmbientTransaction Property

Determines whether the adapter performs the operations on the SQL Server within the context of the ambient
transaction. In BizTalk Server, the same transaction is used to publish/delete messages from the MessageBox.

```csharp
public bool UseAmbientTransaction { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')