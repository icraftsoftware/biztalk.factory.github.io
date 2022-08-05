#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter&lt;TConfig&gt;](WcfNetMsmqAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>')

## WcfNetMsmqAdapter<TConfig>.MsmqSecureHashAlgorithm Property

Specify the hash algorithm to be used for computing the message digest. This property is not available if the [MsmqProtectionLevel](WcfNetMsmqAdapter_TConfig_.MsmqProtectionLevel.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>.MsmqProtectionLevel') property is set to [System.Net.Security.ProtectionLevel.None](https://docs.microsoft.com/en-us/dotnet/api/System.Net.Security.ProtectionLevel.None 'System.Net.Security.ProtectionLevel.None').

```csharp
public System.ServiceModel.MsmqSecureHashAlgorithm MsmqSecureHashAlgorithm { get; set; }
```

Implements [MsmqSecureHashAlgorithm](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqSecurity.MsmqSecureHashAlgorithm 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqSecurity.MsmqSecureHashAlgorithm')

#### Property Value
[System.ServiceModel.MsmqSecureHashAlgorithm](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MsmqSecureHashAlgorithm 'System.ServiceModel.MsmqSecureHashAlgorithm')

### Remarks
It defaults to [System.ServiceModel.MsmqSecureHashAlgorithm.Sha1](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.MsmqSecureHashAlgorithm.Sha1 'System.ServiceModel.MsmqSecureHashAlgorithm.Sha1').