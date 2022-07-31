#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfBasicHttpAdapter&lt;TAddress,TConfig&gt;](WcfBasicHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter<TAddress,TConfig>')

## WcfBasicHttpAdapter<TAddress,TConfig>.SecurityMode Property

Specify the type of security that is used.

```csharp
public System.ServiceModel.BasicHttpSecurityMode SecurityMode { get; set; }
```

Implements [SecurityMode](IAdapterConfigSecurityMode_T_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<T>.SecurityMode')

#### Property Value
[System.ServiceModel.BasicHttpSecurityMode](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpSecurityMode 'System.ServiceModel.BasicHttpSecurityMode')

### Remarks

For more information about the member names for the [SecurityMode](WcfBasicHttpAdapter_TAddress,TConfig_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter<TAddress,TConfig>.SecurityMode') property, see the Security mode
property in [WCF-BasicHttp
            Transport Properties Dialog Box, Receive, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-basichttp-transport-properties-dialog-box-receive-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-basichttp-transport-properties-dialog-box-receive-security-tab') and [WCF-BasicHttp
            Transport Properties Dialog Box, Send, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-basichttp-transport-properties-dialog-box-send-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-basichttp-transport-properties-dialog-box-send-security-tab').

It defaults to [System.ServiceModel.BasicHttpSecurityMode.None](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpSecurityMode.None 'System.ServiceModel.BasicHttpSecurityMode.None').