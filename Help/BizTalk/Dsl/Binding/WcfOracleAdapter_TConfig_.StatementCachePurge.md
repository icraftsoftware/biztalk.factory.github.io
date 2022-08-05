#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter&lt;TConfig&gt;](WcfOracleAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>')

## WcfOracleAdapter<TConfig>.StatementCachePurge Property

Specifies whether the ODP.NET statement cache associated with a connection is purged when the connection is returned
to the connection pool.

```csharp
public bool StatementCachePurge { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

This is an ODP.NET property that is used for performance tuning.

The default is `False`, which disables statement cache purging.