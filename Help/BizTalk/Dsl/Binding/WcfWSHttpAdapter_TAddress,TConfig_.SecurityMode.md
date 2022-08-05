#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWSHttpAdapter&lt;TAddress,TConfig&gt;](WcfWSHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter<TAddress,TConfig>')

## WcfWSHttpAdapter<TAddress,TConfig>.SecurityMode Property

Specify the type of security that is used.

```csharp
public System.ServiceModel.SecurityMode SecurityMode { get; set; }
```

Implements [SecurityMode](IAdapterConfigSecurityMode_T_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<T>.SecurityMode')

#### Property Value
[System.ServiceModel.SecurityMode](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.SecurityMode 'System.ServiceModel.SecurityMode')

### Remarks

For more information about the member names for the [SecurityMode](WcfWSHttpAdapter_TAddress,TConfig_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter<TAddress,TConfig>.SecurityMode') property, see the Security mode
property in [WCF-WSHttp
            Transport Properties Dialog Box, Receive, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-wshttp-transport-properties-dialog-box-receive-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-wshttp-transport-properties-dialog-box-receive-security-tab') and [WCF-WSHttp
            Transport Properties Dialog Box, Send, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-wshttp-transport-properties-dialog-box-send-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-wshttp-transport-properties-dialog-box-send-security-tab').

It defaults to [System.ServiceModel.SecurityMode.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.SecurityMode.Message 'System.ServiceModel.SecurityMode.Message').