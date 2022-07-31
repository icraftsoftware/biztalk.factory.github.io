#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWSHttpAdapter&lt;TAddress,TConfig&gt;](WcfWSHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter<TAddress,TConfig>')

## WcfWSHttpAdapter<TAddress,TConfig>.TransportClientCredentialType Property

Specify the type of credential to be used when performing the client authentication.

```csharp
public System.ServiceModel.HttpClientCredentialType TransportClientCredentialType { get; set; }
```

Implements [TransportClientCredentialType](IAdapterConfigTransportSecurity_T_.TransportClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigTransportSecurity<T>.TransportClientCredentialType')

#### Property Value
[System.ServiceModel.HttpClientCredentialType](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType 'System.ServiceModel.HttpClientCredentialType')

### Remarks

For more information about the member names for the [TransportClientCredentialType](WcfWSHttpAdapter_TAddress,TConfig_.TransportClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter<TAddress,TConfig>.TransportClientCredentialType') property, see the
Transport client credential type property in [WCF-WSHttp
            Transport Properties Dialog Box, Receive, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-wshttp-transport-properties-dialog-box-receive-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-wshttp-transport-properties-dialog-box-receive-security-tab') and [WCF-WSHttp
            Transport Properties Dialog Box, Send, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-wshttp-transport-properties-dialog-box-send-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-wshttp-transport-properties-dialog-box-send-security-tab').

It defaults to [System.ServiceModel.HttpClientCredentialType.Windows](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType.Windows 'System.ServiceModel.HttpClientCredentialType.Windows').