#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfBasicHttpAdapter&lt;TAddress,TConfig&gt;](WcfBasicHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter<TAddress,TConfig>')

## WcfBasicHttpAdapter<TAddress,TConfig>.MessageClientCredentialType Property

Specify the type of credential to be used when performing client authentication using message-based security.

```csharp
public System.ServiceModel.BasicHttpMessageCredentialType MessageClientCredentialType { get; set; }
```

Implements [MessageClientCredentialType](IAdapterConfigMessageSecurity_T_.MessageClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageSecurity<T>.MessageClientCredentialType')

#### Property Value
[System.ServiceModel.BasicHttpMessageCredentialType](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpMessageCredentialType 'System.ServiceModel.BasicHttpMessageCredentialType')

### Remarks

For more information about the member names for the [MessageClientCredentialType](WcfBasicHttpAdapter_TAddress,TConfig_.MessageClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter<TAddress,TConfig>.MessageClientCredentialType') property, see the
Message client credential type property in [WCF-BasicHttp
            Transport Properties Dialog Box, Receive, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-basichttp-transport-properties-dialog-box-receive-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-basichttp-transport-properties-dialog-box-receive-security-tab') and [WCF-BasicHttp
            Transport Properties Dialog Box, Send, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-basichttp-transport-properties-dialog-box-send-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-basichttp-transport-properties-dialog-box-send-security-tab').

It defaults to [System.ServiceModel.BasicHttpMessageCredentialType.UserName](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpMessageCredentialType.UserName 'System.ServiceModel.BasicHttpMessageCredentialType.UserName').