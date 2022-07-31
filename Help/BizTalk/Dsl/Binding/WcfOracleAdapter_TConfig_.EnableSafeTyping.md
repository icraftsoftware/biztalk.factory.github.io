#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter&lt;TConfig&gt;](WcfOracleAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>')

## WcfOracleAdapter<TConfig>.EnableSafeTyping Property

Enables or disables safe typing.

```csharp
public bool EnableSafeTyping { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

This feature controls how the adapter surfaces certain Oracle data types. For more information about safe typing, see
[Basic Oracle Data Types](https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-oracle-database/basic-oracle-data-types1 'https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-oracle-database/basic-oracle-data-types1').

The default is False; safe typing is disabled.