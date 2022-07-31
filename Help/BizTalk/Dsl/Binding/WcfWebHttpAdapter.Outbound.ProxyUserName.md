#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWebHttpAdapter](WcfWebHttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter').[Outbound](WcfWebHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound')

## WcfWebHttpAdapter.Outbound.ProxyUserName Property

Specify the user name to use for the proxy.

```csharp
public string ProxyUserName { get; set; }
```

Implements [ProxyUserName](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigProxySettings.ProxyUserName 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigProxySettings.ProxyUserName')

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

The WCF-BasicHttp adapter leverages the [System.ServiceModel.BasicHttpBinding](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpBinding 'System.ServiceModel.BasicHttpBinding') in the buffered transfer mode to
communicate with an endpoint. Proxy credentials of [System.ServiceModel.BasicHttpBinding](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpBinding 'System.ServiceModel.BasicHttpBinding') are applicable only when the
[SecurityMode](WcfBasicHttpAdapter_TAddress,TConfig_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter<TAddress,TConfig>.SecurityMode') is [System.ServiceModel.BasicHttpSecurityMode.Transport](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpSecurityMode.Transport 'System.ServiceModel.BasicHttpSecurityMode.Transport'),
[System.ServiceModel.BasicHttpSecurityMode.None](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpSecurityMode.None 'System.ServiceModel.BasicHttpSecurityMode.None'), or [System.ServiceModel.BasicHttpSecurityMode.TransportCredentialOnly](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpSecurityMode.TransportCredentialOnly 'System.ServiceModel.BasicHttpSecurityMode.TransportCredentialOnly'). If you
set the [SecurityMode](WcfBasicHttpAdapter_TAddress,TConfig_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter<TAddress,TConfig>.SecurityMode') property to [System.ServiceModel.BasicHttpSecurityMode.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpSecurityMode.Message 'System.ServiceModel.BasicHttpSecurityMode.Message') or [System.ServiceModel.BasicHttpSecurityMode.TransportWithMessageCredential](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpSecurityMode.TransportWithMessageCredential 'System.ServiceModel.BasicHttpSecurityMode.TransportWithMessageCredential'), the
WCF-BasicHttp adapter does not use the credential specified in the [ProxyUserName](WcfWebHttpAdapter.Outbound.ProxyUserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound.ProxyUserName') and [ProxyPassword](WcfWebHttpAdapter.Outbound.ProxyPassword.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound.ProxyPassword') properties for authentication against the proxy.

The WCF-BasicHttp send adapter uses Basic authentication for the proxy.

It defaults to an [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty') string.