#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter&lt;TConfig&gt;](WcfNetMsmqAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>')

## WcfNetMsmqAdapter<TConfig>.MessageClientCredentialType Property

Specify the type of credential to be used when performing client authentication using message-based security.

```csharp
public System.ServiceModel.MessageCredentialType MessageClientCredentialType { get; set; }
```

Implements [MessageClientCredentialType](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqSecurity.MessageClientCredentialType 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqSecurity.MessageClientCredentialType'), [MessageClientCredentialType](IAdapterConfigMessageSecurity_T_.MessageClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageSecurity<T>.MessageClientCredentialType')

#### Property Value
[System.ServiceModel.MessageCredentialType](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType 'System.ServiceModel.MessageCredentialType')

### Remarks

For more information about the member names for the [MessageClientCredentialType](WcfNetMsmqAdapter_TConfig_.MessageClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>.MessageClientCredentialType') property, see the
Message client credential type property in [WCF-NetMsmq
            Transport Properties Dialog Box, Receive, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-netmsmq-transport-properties-dialog-box-receive-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-netmsmq-transport-properties-dialog-box-receive-security-tab').

It defaults to [System.ServiceModel.MessageCredentialType.Windows](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.Windows 'System.ServiceModel.MessageCredentialType.Windows').