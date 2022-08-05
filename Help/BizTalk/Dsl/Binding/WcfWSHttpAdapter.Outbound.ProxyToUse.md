#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWSHttpAdapter](WcfWSHttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter').[Outbound](WcfWSHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter.Outbound')

## WcfWSHttpAdapter.Outbound.ProxyToUse Property

Specify which proxy server to use for outgoing HTTP traffic.

```csharp
public Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection ProxyToUse { get; set; }
```

Implements [ProxyToUse](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigProxyToUse.ProxyToUse 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigProxyToUse.ProxyToUse')

#### Property Value
[Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection 'Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection')

### Remarks
- [Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.None](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.None 'Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.None') — Do not use a proxy server for this send port.
- [Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.Default](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.Default 'Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.Default') — Use the proxy settings in the send handler hosting this send port.
- [Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.UserSpecified](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.UserSpecified 'Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.UserSpecified') — Use the proxy server specified in the [ProxyAddress](WcfWSHttpAdapter.Outbound.ProxyAddress.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter.Outbound.ProxyAddress')
              property.
            It defaults to [Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.None](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.None 'Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.None').