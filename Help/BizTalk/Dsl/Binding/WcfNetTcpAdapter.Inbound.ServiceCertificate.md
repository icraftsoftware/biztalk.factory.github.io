#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetTcpAdapter](WcfNetTcpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter').[Inbound](WcfNetTcpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter.Inbound')

## WcfNetTcpAdapter.Inbound.ServiceCertificate Property

Specify the thumbprint of the X.509 certificate for this receive location that the clients use to authenticate the
service. The certificate to be used for this property must be installed into the My store in the Current User
location.

```csharp
public string ServiceCertificate { get; set; }
```

Implements [ServiceCertificate](IAdapterConfigServiceCertificate.ServiceCertificate.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigServiceCertificate.ServiceCertificate')

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

You must install the service certificate into the Current User location of the user account for the receive
handler hosting this receive location.

It defaults to an [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty') string.