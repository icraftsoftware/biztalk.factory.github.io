#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfCustomAdapter](WcfCustomAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter').[Outbound&lt;TBinding&gt;](WcfCustomAdapter.Outbound_TBinding_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Outbound<TBinding>')

## WcfCustomAdapter.Outbound<TBinding>.ProxyUserName Property

Specify the user name to use for the proxy server specified in the ProxyAddress property. The property is required
if the [ProxyToUse](WcfCustomAdapter.Outbound_TBinding_.ProxyToUse.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Outbound<TBinding>.ProxyToUse') property is set to [Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.UserSpecified](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.UserSpecified 'Microsoft.BizTalk.Adapter.Wcf.Config.ProxySelection.UserSpecified').

```csharp
public string ProxyUserName { get; set; }
```

Implements [ProxyUserName](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigProxySettings.ProxyUserName 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigProxySettings.ProxyUserName')

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
For more information about this property, see [How to Configure a
            WCF-WSHttp Send Port](https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-a-wcf-wshttp-send-port 'https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-a-wcf-wshttp-send-port').