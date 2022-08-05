#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWebHttpAdapter](WcfWebHttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter').[Outbound](WcfWebHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound')

## WcfWebHttpAdapter.Outbound.ProxyAddress Property

Specify the address of the proxy server.

```csharp
public string ProxyAddress { get; set; }
```

Implements [ProxyAddress](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigProxySettings.ProxyAddress 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigProxySettings.ProxyAddress')

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

Use the https or the http scheme depending on the security configuration. This address can be followed by a colon
and the port number. For example, `http://127.0.0.1:8080`.

It defaults to an [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty') string.