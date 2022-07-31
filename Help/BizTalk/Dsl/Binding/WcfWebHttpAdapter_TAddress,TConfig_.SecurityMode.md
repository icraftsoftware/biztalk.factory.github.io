#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWebHttpAdapter&lt;TAddress,TConfig&gt;](WcfWebHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>')

## WcfWebHttpAdapter<TAddress,TConfig>.SecurityMode Property

Specify the type of security that is used.

```csharp
public Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode SecurityMode { get; set; }
```

Implements [SecurityMode](IAdapterConfigSecurityMode_T_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<T>.SecurityMode')

#### Property Value
[Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode 'Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode')

### Remarks

Valid values include the following:
- [Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode.None](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode.None 'Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode.None'): Messages are not secured during
              transfer.
- [Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode.Transport](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode.Transport 'Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode.Transport'): Security is provided using the
              HTTPS transport. The messages are secured using HTTPS. To use this mode, you must set up Secure Sockets Layer (SSL)
              in Microsoft Internet Information Services (IIS).
- [Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode.TransportCredentialOnly](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode.TransportCredentialOnly 'Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode.TransportCredentialOnly'): Integrity,
              confidentiality, and service authentication are provided by the HTTPS transport. To use this mode, you must set up
              Secure Sockets Layer (SSL) in Microsoft Internet Information Services (IIS).

It defaults to [Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode.Transport](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode.Transport 'Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode.Transport').