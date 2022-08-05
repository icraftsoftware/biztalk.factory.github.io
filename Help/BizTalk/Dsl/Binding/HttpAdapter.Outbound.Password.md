#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter').[Outbound](HttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound')

## HttpAdapter.Outbound.Password Property

User password to use for authentication with the server.

```csharp
public string Password { get; set; }
```

Implements [Password](IAdapterConfigOutboundCredentials.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundCredentials.Password')

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
This value is required if you select [Basic](HttpAdapter.AuthenticationScheme.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.AuthenticationScheme.Basic 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.AuthenticationScheme.Basic') or [Digest](HttpAdapter.AuthenticationScheme.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.AuthenticationScheme.Digest 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.AuthenticationScheme.Digest') authentication. The HTTP adapter ignores the value of this
property if [UseSSO](HttpAdapter.Outbound.UseSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.UseSSO') is `True`.