#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter').[Outbound](HttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound')

## HttpAdapter.Outbound.ProxyName Property

Specifies the proxy server name.

```csharp
public string ProxyName { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
The HTTP send adapter ignores this property if the [UseHandlerProxySettings](HttpAdapter.Outbound.UseHandlerProxySettings.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.UseHandlerProxySettings') property is set to
`True`. Otherwise, the HTTP send adapter uses this property only if [UseProxy](HttpAdapter.Outbound.UseProxy.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.UseProxy') is `True`.
This property is required if [UseProxy](HttpAdapter.Outbound.UseProxy.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.UseProxy') is `True`.