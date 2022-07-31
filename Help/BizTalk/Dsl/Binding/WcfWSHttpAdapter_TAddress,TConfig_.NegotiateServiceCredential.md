#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWSHttpAdapter&lt;TAddress,TConfig&gt;](WcfWSHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter<TAddress,TConfig>')

## WcfWSHttpAdapter<TAddress,TConfig>.NegotiateServiceCredential Property

Specify whether the service credential is provisioned at the client out of band, or is obtained from the service to
the client through a process of negotiation. Such a negotiation is a precursor to the usual message exchange.

```csharp
public bool NegotiateServiceCredential { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

If the [MessageClientCredentialType](WcfWSHttpAdapter_TAddress,TConfig_.MessageClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter<TAddress,TConfig>.MessageClientCredentialType') property equals [System.ServiceModel.MessageCredentialType.None](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.None 'System.ServiceModel.MessageCredentialType.None'), [System.ServiceModel.MessageCredentialType.UserName](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.UserName 'System.ServiceModel.MessageCredentialType.UserName'), or [System.ServiceModel.MessageCredentialType.Certificate](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.Certificate 'System.ServiceModel.MessageCredentialType.Certificate'), setting this property to
`False` implies that the service certificate is available at the client out of band and that the client needs to
specify the service certificate. This mode is interoperable with SOAP stacks that implement WS-Trust and
WS-SecureConversation.

If the [MessageClientCredentialType](WcfWSHttpAdapter_TAddress,TConfig_.MessageClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter<TAddress,TConfig>.MessageClientCredentialType') property is set to [System.ServiceModel.MessageCredentialType.Windows](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.Windows 'System.ServiceModel.MessageCredentialType.Windows'),
setting this property to `False` specifies Kerberos-based authentication. This means that the client and service
must be part of the same Kerberos domain. This mode is interoperable with SOAP stacks that implement the Kerberos
token profile (as defined at OASIS WSS TC) as well as WS-Trust and WS-SecureConversation.

When this property is `True`, it causes a .NET SOAP negotiation that tunnels SPNego exchange over SOAP messages.

It defaults to `True`.