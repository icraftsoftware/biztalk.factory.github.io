#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetTcpRelayAdapter](WcfNetTcpRelayAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpRelayAdapter').[Outbound](WcfNetTcpRelayAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpRelayAdapter.Outbound')

## WcfNetTcpRelayAdapter.Outbound.ClientCertificate Property

Specify the thumbprint of the X.509 certificate for authenticating this send port to services. This property is
required if the [MessageClientCredentialType](WcfNetTcpRelayAdapter_TConfig_.MessageClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpRelayAdapter<TConfig>.MessageClientCredentialType') property is set to [System.ServiceModel.MessageCredentialType.Certificate](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MessageCredentialType.Certificate 'System.ServiceModel.MessageCredentialType.Certificate').

```csharp
public string ClientCertificate { get; set; }
```

Implements [ClientCertificate](IAdapterConfigClientCertificate.ClientCertificate.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigClientCertificate.ClientCertificate')

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

The certificate to be used for this property must be installed into the My store in the Current User location of
the user account for the send handler hosting this send port.

It defaults to an [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty') string.