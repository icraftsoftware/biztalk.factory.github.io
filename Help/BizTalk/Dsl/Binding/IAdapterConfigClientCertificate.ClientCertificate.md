#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigClientCertificate](IAdapterConfigClientCertificate.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigClientCertificate')

## IAdapterConfigClientCertificate.ClientCertificate Property

Specify the thumbprint of the X.509 certificate for authenticating this send port to services.

```csharp
string ClientCertificate { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

The certificate to be used for this property must be installed into the My store in the Current User location of the
user account for the send handler hosting this send port.

It defaults to an [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty') string.