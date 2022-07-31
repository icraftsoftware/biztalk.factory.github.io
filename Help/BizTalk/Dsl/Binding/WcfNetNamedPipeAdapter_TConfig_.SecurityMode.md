#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetNamedPipeAdapter&lt;TConfig&gt;](WcfNetNamedPipeAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter<TConfig>')

## WcfNetNamedPipeAdapter<TConfig>.SecurityMode Property

Specify the type of security that is used.

```csharp
public System.ServiceModel.NetNamedPipeSecurityMode SecurityMode { get; set; }
```

Implements [SecurityMode](IAdapterConfigSecurityMode_T_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<T>.SecurityMode')

#### Property Value
[System.ServiceModel.NetNamedPipeSecurityMode](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.NetNamedPipeSecurityMode 'System.ServiceModel.NetNamedPipeSecurityMode')

### Remarks
- [System.ServiceModel.NetNamedPipeSecurityMode.None](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.NetNamedPipeSecurityMode.None 'System.ServiceModel.NetNamedPipeSecurityMode.None') — This disables security.
- [System.ServiceModel.NetNamedPipeSecurityMode.Transport](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.NetNamedPipeSecurityMode.Transport 'System.ServiceModel.NetNamedPipeSecurityMode.Transport') — Security is provided using underlying transport-based
              security. It is possible to control the protection level with this mode.