#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter&lt;TConfig&gt;](WcfOracleAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>')

## WcfOracleAdapter<TConfig>.DataFetchSize Property

Specifies the amount of data in bytes that ODP.NET fetches from the result set in one server round-trip.

```csharp
public long DataFetchSize { get; set; }
```

#### Property Value
[System.Int64](https://docs.microsoft.com/en-us/dotnet/api/System.Int64 'System.Int64')

### Remarks

This is an ODP.NET property that is used for performance tuning.

It defaults to 65536, roughly [UInt16.MaxValue](https://docs.microsoft.com/en-us/dotnet/api/System.UInt16.MaxValue 'System.UInt16.MaxValue').