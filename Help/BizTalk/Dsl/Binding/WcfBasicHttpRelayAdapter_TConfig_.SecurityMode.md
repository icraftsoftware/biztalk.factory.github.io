#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfBasicHttpRelayAdapter&lt;TConfig&gt;](WcfBasicHttpRelayAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>')

## WcfBasicHttpRelayAdapter<TConfig>.SecurityMode Property

Specify the type of security that is used.

```csharp
public Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode SecurityMode { get; set; }
```

Implements [SecurityMode](IAdapterConfigSecurityMode_T_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<T>.SecurityMode')

#### Property Value
[Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode 'Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode')

### Remarks

Valid values include the following:
- [Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode.None](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode.None 'Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode.None') — Messages are not secured during transfer.
- [Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode.Transport](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode.Transport 'Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode.Transport') — Security is provided using the HTTPS transport. The SOAP messages are secured using HTTPS. To use this mode, you must
  set up Secure Sockets Layer (SSL) in Microsoft Internet Information Services (IIS).
- [Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode.Message](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode.Message 'Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode.Message') — Security is provided using SOAP message security over the HTTP transport. By default, the SOAP Body is encrypted and
  signed. The only valid Message client credential type for the WCF-Basic adapter is Certificate. This mode requires
  the HTTP transport. When using this security mode, the service certificate for this receive location needs to be
  provided through the Service certificate - Thumbprint property.
- [Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode.TransportWithMessageCredential](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode.TransportWithMessageCredential 'Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode.TransportWithMessageCredential') — Integrity, confidentiality, and service authentication are provided by the HTTPS transport. To use this mode, you
  must set up Secure Sockets Layer (SSL) in Microsoft Internet Information Services (IIS).

It defaults to [Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode.Transport](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode.Transport 'Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode.Transport').