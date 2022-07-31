#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter&lt;TConfig&gt;](WcfNetMsmqAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>')

## WcfNetMsmqAdapter<TConfig>.SecurityMode Property

Specify the type of security that is used.

```csharp
public System.ServiceModel.NetMsmqSecurityMode SecurityMode { get; set; }
```

Implements [SecurityMode](IAdapterConfigSecurityMode_T_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<T>.SecurityMode'), [SecurityMode](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqSecurity.SecurityMode 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqSecurity.SecurityMode')

#### Property Value
[System.ServiceModel.NetMsmqSecurityMode](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.NetMsmqSecurityMode 'System.ServiceModel.NetMsmqSecurityMode')

### Remarks

For more information about the member names for the [SecurityMode](WcfNetMsmqAdapter_TConfig_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>.SecurityMode') property, see the Security mode
property in [WCF-NetMsmq
            Transport Properties Dialog Box, Receive, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-netmsmq-transport-properties-dialog-box-receive-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-netmsmq-transport-properties-dialog-box-receive-security-tab').

It defaults to [System.ServiceModel.NetMsmqSecurityMode.Transport](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.NetMsmqSecurityMode.Transport 'System.ServiceModel.NetMsmqSecurityMode.Transport').