#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfCustomAdapter](WcfCustomAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter').[Outbound&lt;TBinding&gt;](WcfCustomAdapter.Outbound_TBinding_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Outbound<TBinding>')

## WcfCustomAdapter.Outbound<TBinding>.ProxyAddress Property

Specify the address of the proxy server. Use the <b>https</b> or the http scheme depending on the security
configuration. This address can be followed by a colon and the port number. The property is required if the [ProxyToUse](WcfCustomAdapter.Outbound_TBinding_.ProxyToUse.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Outbound<TBinding>.ProxyToUse') property is set to [Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.UserSpecified](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.UserSpecified 'Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.UserSpecified').

```csharp
public string ProxyAddress { get; set; }
```

Implements [ProxyAddress](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigProxySettings.ProxyAddress 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigProxySettings.ProxyAddress')

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
It defaults to [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty').