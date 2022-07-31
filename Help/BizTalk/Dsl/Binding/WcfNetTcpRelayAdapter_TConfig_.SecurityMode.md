#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetTcpRelayAdapter&lt;TConfig&gt;](WcfNetTcpRelayAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpRelayAdapter<TConfig>')

## WcfNetTcpRelayAdapter<TConfig>.SecurityMode Property

Specify the type of security that is used.

```csharp
public Microsoft.ServiceBus.EndToEndSecurityMode SecurityMode { get; set; }
```

Implements [SecurityMode](IAdapterConfigSecurityMode_T_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<T>.SecurityMode')

#### Property Value
[Microsoft.ServiceBus.EndToEndSecurityMode](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.EndToEndSecurityMode 'Microsoft.ServiceBus.EndToEndSecurityMode')

### Remarks

Valid values include the following:
- [Microsoft.ServiceBus.EndToEndSecurityMode.None](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.EndToEndSecurityMode.None 'Microsoft.ServiceBus.EndToEndSecurityMode.None') — Messages are not secured during transfer.
- [Microsoft.ServiceBus.EndToEndSecurityMode.Message](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.EndToEndSecurityMode.Message 'Microsoft.ServiceBus.EndToEndSecurityMode.Message') — Security is provided using SOAP message security. By default, the SOAP Body is encrypted and signed. This mode offers
  a variety of features, such as whether the service credentials are available at the client out of band, and the
  algorithm suite to use. If you select [System.ServiceModel.MessageCredentialType.None](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.None 'System.ServiceModel.MessageCredentialType.None'), [System.ServiceModel.MessageCredentialType.UserName](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.UserName 'System.ServiceModel.MessageCredentialType.UserName'), or [System.ServiceModel.MessageCredentialType.Certificate](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.Certificate 'System.ServiceModel.MessageCredentialType.Certificate') for the [MessageClientCredentialType](WcfNetTcpRelayAdapter_TConfig_.MessageClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpRelayAdapter<TConfig>.MessageClientCredentialType') property in this security mode, you must supply the service certificate for this
  receive location through the [WCF.ServiceCertificate](https://docs.microsoft.com/en-us/dotnet/api/WCF.ServiceCertificate 'WCF.ServiceCertificate') thumbprint property.
- [Microsoft.ServiceBus.EndToEndSecurityMode.Transport](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.EndToEndSecurityMode.Transport 'Microsoft.ServiceBus.EndToEndSecurityMode.Transport') — Transport security is provided using TLS over TCP or SPNego. It is possible to control the protection level with this
  mode. If you select If you select [System.ServiceModel.MessageCredentialType.None](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.None 'System.ServiceModel.MessageCredentialType.None') or [System.ServiceModel.MessageCredentialType.Certificate](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.Certificate 'System.ServiceModel.MessageCredentialType.Certificate') for the [MessageClientCredentialType](WcfNetTcpRelayAdapter_TConfig_.MessageClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpRelayAdapter<TConfig>.MessageClientCredentialType') property in this
  security mode, you must supply the service certificate for this receive location through the [WCF.ServiceCertificate](https://docs.microsoft.com/en-us/dotnet/api/WCF.ServiceCertificate 'WCF.ServiceCertificate') thumbprint property.
- [Microsoft.ServiceBus.EndToEndSecurityMode.TransportWithMessageCredential](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.EndToEndSecurityMode.TransportWithMessageCredential 'Microsoft.ServiceBus.EndToEndSecurityMode.TransportWithMessageCredential') — Transport security is coupled with message security. Transport security is provided by TLS over TCP or SPNego and
  ensures integrity, confidentiality, and server authentication. If you select [System.ServiceModel.MessageCredentialType.Windows](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.Windows 'System.ServiceModel.MessageCredentialType.Windows'), [System.ServiceModel.MessageCredentialType.UserName](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.UserName 'System.ServiceModel.MessageCredentialType.UserName'), or [System.ServiceModel.MessageCredentialType.Certificate](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.Certificate 'System.ServiceModel.MessageCredentialType.Certificate') for the [MessageClientCredentialType](WcfNetTcpRelayAdapter_TConfig_.MessageClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpRelayAdapter<TConfig>.MessageClientCredentialType') property in this
  security mode, you must supply the service certificate for this receive location through the [WCF.ServiceCertificate](https://docs.microsoft.com/en-us/dotnet/api/WCF.ServiceCertificate 'WCF.ServiceCertificate') thumbprint property.

It defaults to [Microsoft.ServiceBus.EndToEndSecurityMode.Transport](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.EndToEndSecurityMode.Transport 'Microsoft.ServiceBus.EndToEndSecurityMode.Transport').