#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter').[Outbound](HttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound')

## HttpAdapter.Outbound.ProxyPassword Property

Specifies the user password for authentication with the proxy server.

```csharp
public string ProxyPassword { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
The HTTP send adapter ignores this property if [UseHandlerProxySettings](HttpAdapter.Outbound.UseHandlerProxySettings.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.UseHandlerProxySettings') is `True`. Otherwise,
HTTP send adapter uses this property only if [UseProxy](HttpAdapter.Outbound.UseProxy.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.UseProxy') is `True`.