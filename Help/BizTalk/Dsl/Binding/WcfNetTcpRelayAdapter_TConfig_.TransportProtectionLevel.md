#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetTcpRelayAdapter&lt;TConfig&gt;](WcfNetTcpRelayAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpRelayAdapter<TConfig>')

## WcfNetTcpRelayAdapter<TConfig>.TransportProtectionLevel Property

Define security at the level of the TCP transport.

```csharp
public System.Net.Security.ProtectionLevel TransportProtectionLevel { get; set; }
```

#### Property Value
[System.Net.Security.ProtectionLevel](https://docs.microsoft.com/en-us/dotnet/api/System.Net.Security.ProtectionLevel 'System.Net.Security.ProtectionLevel')

### Remarks

Signing messages mitigates the risk of a third party tampering with the message while it is being transferred.
Encryption provides data-level privacy during transport.

Valid values include the following:
- [System.Net.Security.ProtectionLevel.None](https://docs.microsoft.com/en-us/dotnet/api/System.Net.Security.ProtectionLevel.None 'System.Net.Security.ProtectionLevel.None') — No protection.
- [System.Net.Security.ProtectionLevel.Sign](https://docs.microsoft.com/en-us/dotnet/api/System.Net.Security.ProtectionLevel.Sign 'System.Net.Security.ProtectionLevel.Sign') — Messages are signed.
- [System.Net.Security.ProtectionLevel.EncryptAndSign](https://docs.microsoft.com/en-us/dotnet/api/System.Net.Security.ProtectionLevel.EncryptAndSign 'System.Net.Security.ProtectionLevel.EncryptAndSign') — Messages are encrypted and signed.

It defaults to [System.Net.Security.ProtectionLevel.EncryptAndSign](https://docs.microsoft.com/en-us/dotnet/api/System.Net.Security.ProtectionLevel.EncryptAndSign 'System.Net.Security.ProtectionLevel.EncryptAndSign').