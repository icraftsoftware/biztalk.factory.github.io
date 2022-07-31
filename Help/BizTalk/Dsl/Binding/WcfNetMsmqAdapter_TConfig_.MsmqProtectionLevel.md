#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter&lt;TConfig&gt;](WcfNetMsmqAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>')

## WcfNetMsmqAdapter<TConfig>.MsmqProtectionLevel Property

Specify the way messages are secured at the level of the MSMQ transport. Encryption ensures message integrity, while
sign and encrypt ensures both message integrity and non-repudiation.

```csharp
public System.Net.Security.ProtectionLevel MsmqProtectionLevel { get; set; }
```

Implements [MsmqProtectionLevel](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqSecurity.MsmqProtectionLevel 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqSecurity.MsmqProtectionLevel')

#### Property Value
[System.Net.Security.ProtectionLevel](https://docs.microsoft.com/en-us/dotnet/api/System.Net.Security.ProtectionLevel 'System.Net.Security.ProtectionLevel')

### Remarks

- [System.Net.Security.ProtectionLevel.None](https://docs.microsoft.com/en-us/dotnet/api/System.Net.Security.ProtectionLevel.None 'System.Net.Security.ProtectionLevel.None') — No protection.
- [System.Net.Security.ProtectionLevel.Sign](https://docs.microsoft.com/en-us/dotnet/api/System.Net.Security.ProtectionLevel.Sign 'System.Net.Security.ProtectionLevel.Sign') — Messages are signed.
- [System.Net.Security.ProtectionLevel.EncryptAndSign](https://docs.microsoft.com/en-us/dotnet/api/System.Net.Security.ProtectionLevel.EncryptAndSign 'System.Net.Security.ProtectionLevel.EncryptAndSign') — Messages are encrypted and signed. To use this protection level,
              you must enable Active Directory Integration for MSMQ.

It defaults to [System.Net.Security.ProtectionLevel.Sign](https://docs.microsoft.com/en-us/dotnet/api/System.Net.Security.ProtectionLevel.Sign 'System.Net.Security.ProtectionLevel.Sign').