#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter&lt;TConfig&gt;](WcfNetMsmqAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>')

## WcfNetMsmqAdapter<TConfig>.MsmqAuthenticationMode Property

Specify how the message must be authenticated by the MSMQ transport.

```csharp
public System.ServiceModel.MsmqAuthenticationMode MsmqAuthenticationMode { get; set; }
```

Implements [MsmqAuthenticationMode](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqSecurity.MsmqAuthenticationMode 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqSecurity.MsmqAuthenticationMode')

#### Property Value
[System.ServiceModel.MsmqAuthenticationMode](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MsmqAuthenticationMode 'System.ServiceModel.MsmqAuthenticationMode')

### Remarks

For more information about the member names for the [MsmqAuthenticationMode](WcfNetMsmqAdapter_TConfig_.MsmqAuthenticationMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>.MsmqAuthenticationMode') property, see the MSMQ
authentication mode property in [WCF-NetMsmq
            Transport Properties Dialog Box, Receive, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-netmsmq-transport-properties-dialog-box-receive-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-netmsmq-transport-properties-dialog-box-receive-security-tab').

It defaults to [System.ServiceModel.MsmqAuthenticationMode.WindowsDomain](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MsmqAuthenticationMode.WindowsDomain 'System.ServiceModel.MsmqAuthenticationMode.WindowsDomain').