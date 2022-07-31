#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter&lt;TConfig&gt;](WcfOracleAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>')

## WcfOracleAdapter<TConfig>.LongDataTypeColumnSize Property

Specifies the maximum size in bytes (32512) of an Oracle long data type column.

```csharp
public long LongDataTypeColumnSize { get; set; }
```

#### Property Value
[System.Int64](https://docs.microsoft.com/en-us/dotnet/api/System.Int64 'System.Int64')

### Remarks
The default is 0. You must use the default value if you are not performing operation on long data type. To prefetch
the data, you must specify -1 as the value for this binding property. You must explicitly set an appropriate value
for this binding property if you are:
- Executing a stored procedure that contains parameters of long data type.
- Performing a Select operation on a table that contains columns with long data type, and the SELECT statement does not
  include the primary key column.
This binding property is deprecated and should be set only if Long data type is used.