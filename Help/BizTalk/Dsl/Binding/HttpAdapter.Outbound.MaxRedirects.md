#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter').[Outbound](HttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound')

## HttpAdapter.Outbound.MaxRedirects Property

Maximum number of times that the HTTP adapter can redirect the request.

```csharp
public int MaxRedirects { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks
It defaults to `5`. Values between `0` and `10` are accepted.