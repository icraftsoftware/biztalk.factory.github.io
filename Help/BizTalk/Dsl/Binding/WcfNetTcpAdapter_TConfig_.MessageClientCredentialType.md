#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetTcpAdapter&lt;TConfig&gt;](WcfNetTcpAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter<TConfig>')

## WcfNetTcpAdapter<TConfig>.MessageClientCredentialType Property

Specify the type of credential to be used when performing client authentication using message-based security.

```csharp
public System.ServiceModel.MessageCredentialType MessageClientCredentialType { get; set; }
```

Implements [MessageClientCredentialType](IAdapterConfigMessageSecurity_T_.MessageClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageSecurity<T>.MessageClientCredentialType')

#### Property Value
[System.ServiceModel.MessageCredentialType](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType 'System.ServiceModel.MessageCredentialType')

### Remarks

For more information about the member names for the [System.ServiceModel.MessageCredentialType](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType 'System.ServiceModel.MessageCredentialType') property, see the Message
client credential type property in [WCF-NetTcp
            Transport Properties Dialog Box, Receive, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-nettcp-transport-properties-dialog-box-receive-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-nettcp-transport-properties-dialog-box-receive-security-tab').

It defaults to [System.ServiceModel.MessageCredentialType.Windows](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.Windows 'System.ServiceModel.MessageCredentialType.Windows').