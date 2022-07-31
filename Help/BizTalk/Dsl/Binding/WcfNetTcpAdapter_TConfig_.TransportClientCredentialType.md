#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetTcpAdapter&lt;TConfig&gt;](WcfNetTcpAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter<TConfig>')

## WcfNetTcpAdapter<TConfig>.TransportClientCredentialType Property

Specify the type of credential to be used when performing the client authentication.

```csharp
public System.ServiceModel.TcpClientCredentialType TransportClientCredentialType { get; set; }
```

Implements [TransportClientCredentialType](IAdapterConfigTransportSecurity_T_.TransportClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigTransportSecurity<T>.TransportClientCredentialType')

#### Property Value
[System.ServiceModel.TcpClientCredentialType](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.TcpClientCredentialType 'System.ServiceModel.TcpClientCredentialType')

### Remarks

For more information about the member names for the [TransportClientCredentialType](WcfNetTcpAdapter_TConfig_.TransportClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter<TConfig>.TransportClientCredentialType') property, see the
Transport client credential type property in [WCF-NetTcp
            Transport Properties Dialog Box, Receive, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-nettcp-transport-properties-dialog-box-receive-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-nettcp-transport-properties-dialog-box-receive-security-tab').

It defaults to [System.ServiceModel.TcpClientCredentialType.Windows](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.TcpClientCredentialType.Windows 'System.ServiceModel.TcpClientCredentialType.Windows').