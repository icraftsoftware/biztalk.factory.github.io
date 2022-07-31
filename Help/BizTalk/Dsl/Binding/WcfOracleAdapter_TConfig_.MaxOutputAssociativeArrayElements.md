#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter&lt;TConfig&gt;](WcfOracleAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>')

## WcfOracleAdapter<TConfig>.MaxOutputAssociativeArrayElements Property

Specifies the size of the associate array that the adapter creates when performing operations that return an
associative array in the response. The adapter communicates the size of the array to ODP.NET, which in turn creates a
buffer depending on the array size.

```csharp
public int MaxOutputAssociativeArrayElements { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks

This binding property is useful when performing operations involving PL/SQL table types.

It defaults to 32.