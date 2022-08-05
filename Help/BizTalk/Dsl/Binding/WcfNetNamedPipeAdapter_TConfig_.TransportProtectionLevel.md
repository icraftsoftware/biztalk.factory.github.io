#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetNamedPipeAdapter&lt;TConfig&gt;](WcfNetNamedPipeAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter<TConfig>')

## WcfNetNamedPipeAdapter<TConfig>.TransportProtectionLevel Property

Define security at the level of the TCP transport. Signing messages mitigates the risk of a third party tampering
with the message while it is being transferred. Encryption provides data-level privacy during transport.

```csharp
public System.Net.Security.ProtectionLevel TransportProtectionLevel { get; set; }
```

#### Property Value
[System.Net.Security.ProtectionLevel](https://docs.microsoft.com/en-us/dotnet/api/System.Net.Security.ProtectionLevel 'System.Net.Security.ProtectionLevel')

### Remarks
It defaults to [System.Net.Security.ProtectionLevel.EncryptAndSign](https://docs.microsoft.com/en-us/dotnet/api/System.Net.Security.ProtectionLevel.EncryptAndSign 'System.Net.Security.ProtectionLevel.EncryptAndSign').