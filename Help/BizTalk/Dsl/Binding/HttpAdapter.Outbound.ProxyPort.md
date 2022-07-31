#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter').[Outbound](HttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound')

## HttpAdapter.Outbound.ProxyPort Property

Specifies the proxy server port.

```csharp
public int ProxyPort { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks

The HTTP send adapter ignores this property if [UseHandlerProxySettings](HttpAdapter.Outbound.UseHandlerProxySettings.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.UseHandlerProxySettings') is `True`. Otherwise,
HTTP send adapter uses this property only if [UseProxy](HttpAdapter.Outbound.UseProxy.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.UseProxy') is `True`. This property is required if
[UseProxy](HttpAdapter.Outbound.UseProxy.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.UseProxy') is `True`.

Values between `0` and `65535` are accepted.