#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetTcpAdapter&lt;TConfig&gt;](WcfNetTcpAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter<TConfig>')

## WcfNetTcpAdapter<TConfig>.SecurityMode Property

Specify the type of security that is used.

```csharp
public System.ServiceModel.SecurityMode SecurityMode { get; set; }
```

Implements [SecurityMode](IAdapterConfigSecurityMode_T_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<T>.SecurityMode')

#### Property Value
[System.ServiceModel.SecurityMode](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.SecurityMode 'System.ServiceModel.SecurityMode')

### Remarks

For more information about the member names for the [SecurityMode](WcfNetTcpAdapter_TConfig_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter<TConfig>.SecurityMode') property, see the Security mode
property in [WCF-NetTcp
            Transport Properties Dialog Box, Send, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-nettcp-transport-properties-dialog-box-send-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-nettcp-transport-properties-dialog-box-send-security-tab').

It defaults to [System.ServiceModel.SecurityMode.Transport](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.SecurityMode.Transport 'System.ServiceModel.SecurityMode.Transport').