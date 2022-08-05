#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FileAdapter](FileAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter').[Outbound](FileAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Outbound')

## FileAdapter.Outbound.UseTempFileOnWrite Property

Use temporary file while writing.

```csharp
public bool UseTempFileOnWrite { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks
Can be set to `true` only when the [Mode](FileAdapter.Outbound.Mode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Outbound.Mode') is set to [CreateNew](FileAdapter.CopyMode.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.CopyMode.CreateNew 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.CopyMode.CreateNew').