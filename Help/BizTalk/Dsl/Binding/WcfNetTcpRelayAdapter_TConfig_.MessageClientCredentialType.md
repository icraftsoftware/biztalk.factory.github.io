#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetTcpRelayAdapter&lt;TConfig&gt;](WcfNetTcpRelayAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpRelayAdapter<TConfig>')

## WcfNetTcpRelayAdapter<TConfig>.MessageClientCredentialType Property

Specify the type of credential to be used when performing client authentication using message-based security.

```csharp
public System.ServiceModel.MessageCredentialType MessageClientCredentialType { get; set; }
```

Implements [MessageClientCredentialType](IAdapterConfigMessageSecurity_T_.MessageClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageSecurity<T>.MessageClientCredentialType')

#### Property Value
[System.ServiceModel.MessageCredentialType](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType 'System.ServiceModel.MessageCredentialType')

### Remarks

This is required only if the Security mode is set to Message or TransportWithMessageCredential.

Valid values include the following:
- [System.ServiceModel.MessageCredentialType.None](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.None 'System.ServiceModel.MessageCredentialType.None') — This allows the service to interact with anonymous clients. This indicates that this client does not provide any
  client credential.
- [System.ServiceModel.MessageCredentialType.Certificate](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.Certificate 'System.ServiceModel.MessageCredentialType.Certificate') — Clients are authenticated to this receive location using the client certificate specified through [WCF.ServiceCertificate](https://docs.microsoft.com/en-us/dotnet/api/WCF.ServiceCertificate 'WCF.ServiceCertificate') thumbprint property. The credential is passed through the SOAP Header element using the
  WSS SOAP Message Security X509 Token Profile 1.0 protocol. To authenticate the client certificates, the CA
  certificate chain for the client certificates must be installed in the Trusted Root Certification Authorities
  certificate store of this computer.
- [System.ServiceModel.MessageCredentialType.UserName](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.UserName 'System.ServiceModel.MessageCredentialType.UserName') — Clients are authenticated to this receive location with a UserName credential. The credential is passed through the
  SOAP Header element using the WSS SOAP Message Security UsernameToken Profile 1.0 protocol. You must create the
  domain or local user accounts corresponding to client credentials.
- [System.ServiceModel.MessageCredentialType.Windows](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.Windows 'System.ServiceModel.MessageCredentialType.Windows') — Allow the SOAP exchanges to be under the authenticated context of a Windows credential. The client credential is
  passed through the SOAP Header element using the WSS SOAP Message Security Kerberos Token Profile 1.0 protocol. You
  must create the domain or local user accounts corresponding to client credentials. In addition, the client's
  userPrincipalName element must be configured with the user account name running this receive handler.

It defaults to [System.ServiceModel.MessageCredentialType.Windows](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.Windows 'System.ServiceModel.MessageCredentialType.Windows').