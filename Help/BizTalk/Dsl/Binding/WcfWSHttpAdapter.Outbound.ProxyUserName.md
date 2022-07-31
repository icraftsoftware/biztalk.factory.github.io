#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWSHttpAdapter](WcfWSHttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter').[Outbound](WcfWSHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter.Outbound')

## WcfWSHttpAdapter.Outbound.ProxyUserName Property

Specify the user name to use for the proxy.

```csharp
public string ProxyUserName { get; set; }
```

Implements [ProxyUserName](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigProxySettings.ProxyUserName 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigProxySettings.ProxyUserName')

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

The WCF-WSHttp adapter leverages the [System.ServiceModel.WSHttpBinding](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.WSHttpBinding 'System.ServiceModel.WSHttpBinding') in the buffered transfer mode to communicate with
an endpoint. Proxy credentials of [System.ServiceModel.WSHttpBinding](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.WSHttpBinding 'System.ServiceModel.WSHttpBinding') are applicable only when the [SecurityMode](WcfWSHttpAdapter_TAddress,TConfig_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter<TAddress,TConfig>.SecurityMode') is [System.ServiceModel.SecurityMode.Transport](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.SecurityMode.Transport 'System.ServiceModel.SecurityMode.Transport') or [System.ServiceModel.SecurityMode.None](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.SecurityMode.None 'System.ServiceModel.SecurityMode.None'). If you set the [SecurityMode](WcfWSHttpAdapter_TAddress,TConfig_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter<TAddress,TConfig>.SecurityMode') property
to
[System.ServiceModel.SecurityMode.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.SecurityMode.Message 'System.ServiceModel.SecurityMode.Message')
or [System.ServiceModel.SecurityMode.TransportWithMessageCredential](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.SecurityMode.TransportWithMessageCredential 'System.ServiceModel.SecurityMode.TransportWithMessageCredential'), the WCF-WSHttp adapter does not use the credential
specified in the [ProxyUserName](WcfWSHttpAdapter.Outbound.ProxyUserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter.Outbound.ProxyUserName') and [ProxyPassword](WcfWSHttpAdapter.Outbound.ProxyPassword.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter.Outbound.ProxyPassword') properties for authentication against
the proxy.

The WCF-WSHttp send adapter uses Basic authentication for the proxy.

It defaults to an [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty') string.