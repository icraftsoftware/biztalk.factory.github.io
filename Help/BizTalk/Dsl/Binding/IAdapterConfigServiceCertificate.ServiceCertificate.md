#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigServiceCertificate](IAdapterConfigServiceCertificate.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigServiceCertificate')

## IAdapterConfigServiceCertificate.ServiceCertificate Property

Specify the thumbprint of the X.509 certificate that a receive location or send port uses to authenticate the
service.

```csharp
string ServiceCertificate { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
- Inbound — Specify the thumbprint of the X.509 certificate for this receive location that the clients use to
  authenticate the service. The certificate to be used for this property must be installed into the My store in the
  Current User location.
- Outbound — Specify the thumbprint of the X.509 certificate for authenticating the service to which this send
  port sends messages. The certificate to be used for this property must be installed into the Other People store in
  the Local Machine location.
            It defaults to an [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty') string.