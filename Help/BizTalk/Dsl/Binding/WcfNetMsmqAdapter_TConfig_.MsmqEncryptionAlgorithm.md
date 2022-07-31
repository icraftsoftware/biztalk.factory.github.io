#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter&lt;TConfig&gt;](WcfNetMsmqAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>')

## WcfNetMsmqAdapter<TConfig>.MsmqEncryptionAlgorithm Property

Specify the algorithm to be used for message encryption on the wire when transferring messages between message queue
managers. This property is available only if the [MsmqProtectionLevel](WcfNetMsmqAdapter_TConfig_.MsmqProtectionLevel.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>.MsmqProtectionLevel') property is set to [System.Net.Security.ProtectionLevel.EncryptAndSign](https://docs.microsoft.com/en-us/dotnet/api/System.Net.Security.ProtectionLevel.EncryptAndSign 'System.Net.Security.ProtectionLevel.EncryptAndSign').

```csharp
public System.ServiceModel.MsmqEncryptionAlgorithm MsmqEncryptionAlgorithm { get; set; }
```

Implements [MsmqEncryptionAlgorithm](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqSecurity.MsmqEncryptionAlgorithm 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqSecurity.MsmqEncryptionAlgorithm')

#### Property Value
[System.ServiceModel.MsmqEncryptionAlgorithm](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MsmqEncryptionAlgorithm 'System.ServiceModel.MsmqEncryptionAlgorithm')

### Remarks
It defaults to [System.ServiceModel.MsmqEncryptionAlgorithm.RC4Stream](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MsmqEncryptionAlgorithm.RC4Stream 'System.ServiceModel.MsmqEncryptionAlgorithm.RC4Stream').