#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWebHttpAdapter&lt;TAddress,TConfig&gt;](WcfWebHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>')

## WcfWebHttpAdapter<TAddress,TConfig>.TransportClientCredentialType Property

Specify the type of credential to be used when performing the client authentication.

```csharp
public System.ServiceModel.HttpClientCredentialType TransportClientCredentialType { get; set; }
```

Implements [TransportClientCredentialType](IAdapterConfigTransportSecurity_T_.TransportClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigTransportSecurity<T>.TransportClientCredentialType')

#### Property Value
[System.ServiceModel.HttpClientCredentialType](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType 'System.ServiceModel.HttpClientCredentialType')

### Remarks

Valid values include the following:
- [System.ServiceModel.HttpClientCredentialType.None](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType.None 'System.ServiceModel.HttpClientCredentialType.None'): No authentication occurs at the transport level.
- [System.ServiceModel.HttpClientCredentialType.Basic](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType.Basic 'System.ServiceModel.HttpClientCredentialType.Basic'): Basic authentication. In Basic authentication, user names and passwords
              are sent in plain text over the network. You must create the domain or local user accounts corresponding to the
              credentials.
- [System.ServiceModel.HttpClientCredentialType.Digest](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType.Digest 'System.ServiceModel.HttpClientCredentialType.Digest'): Digest authentication. This authentication method operates much like
              Basic authentication, except that passwords are sent across the network as a hash value for additional security.
              Digest authentication is available only on domains with domain controllers running Windows Server operating systems
              authentication. You must create the domain or local user accounts corresponding to client credentials.
- [System.ServiceModel.HttpClientCredentialType.Ntlm](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType.Ntlm 'System.ServiceModel.HttpClientCredentialType.Ntlm'): NTLM authentication. Clients can send the credentials without sending a
              password to this receive location. You must create the domain or local user accounts corresponding to client
              credentials.
- [System.ServiceModel.HttpClientCredentialType.Windows](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType.Windows 'System.ServiceModel.HttpClientCredentialType.Windows'): Windows integrated authentication. Windows Communication Foundation
              negotiates Kerberos or NTLM, preferring Kerberos if a domain is present. If you want to use Kerberos it is important
              to have the client identify the service with a service principal name (SPN). You must create the domain or local user
              accounts corresponding to client credentials.
- [System.ServiceModel.HttpClientCredentialType.Certificate](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType.Certificate 'System.ServiceModel.HttpClientCredentialType.Certificate'): Client authentication using the client certificate. The CA
              certificate chain for the client X.509 certificates must be installed in the Trusted Root Certification Authorities
              certificate store of this computer so that the clients can be authenticated to this receive location.

The Transport client credential type property must match the authentication scheme of the IIS virtual directory
hosting this receive location. For example, if the property is set to Windows, you also need to enable Integrated
Windows authentication for the virtual directory that hosts it. Similarly if the property is set to None, you must
allow anonymous access to the virtual directory that hosts this receive location.

It defaults to [System.ServiceModel.HttpClientCredentialType.Windows](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType.Windows 'System.ServiceModel.HttpClientCredentialType.Windows').