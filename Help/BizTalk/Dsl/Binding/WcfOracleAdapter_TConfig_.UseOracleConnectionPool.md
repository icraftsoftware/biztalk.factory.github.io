#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter&lt;TConfig&gt;](WcfOracleAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>')

## WcfOracleAdapter<TConfig>.UseOracleConnectionPool Property

Specifies whether to use the ODP.NET connection pool. The Oracle Database adapter implements connection pooling by
using the ODP.NET connection pool.

```csharp
public bool UseOracleConnectionPool { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks
The default is `True`, which enables connection pooling.