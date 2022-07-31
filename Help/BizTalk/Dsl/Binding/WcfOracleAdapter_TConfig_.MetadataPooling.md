#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter&lt;TConfig&gt;](WcfOracleAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>')

## WcfOracleAdapter<TConfig>.MetadataPooling Property

Specifies whether ODP.NET caches metadata information for executed queries.

```csharp
public bool MetadataPooling { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

This is an ODP.NET property that is used for performance tuning. Caching metadata information improves performance;
however, if changes to the underlying Oracle artifacts occur on the Oracle system, this pooled metadata will be out
of sync. This might cause operations performed on the Oracle system to return unexpected exceptions.

The default is `True`, which enables metadata pooling.