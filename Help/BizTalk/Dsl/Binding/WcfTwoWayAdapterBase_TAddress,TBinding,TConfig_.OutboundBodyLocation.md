#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfTwoWayAdapterBase&lt;TAddress,TBinding,TConfig&gt;](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>')

## WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>.OutboundBodyLocation Property

Specify the data selection for the SOAP Body element of outgoing WCF messages.

```csharp
public Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection OutboundBodyLocation { get; set; }
```

Implements [OutboundBodyLocation](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOutboundMessageMarshalling.OutboundBodyLocation 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOutboundMessageMarshalling.OutboundBodyLocation')

#### Property Value
[Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection 'Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection')

### Remarks

- [Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseBodyElement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseBodyElement 'Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseBodyElement') — Use the BizTalk message body part to create the
              content of the SOAP Body element for an outgoing message.
- [Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseTemplate](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseTemplate 'Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseTemplate') — Use the template supplied in the [OutboundXmlTemplate](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.OutboundXmlTemplate.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>.OutboundXmlTemplate') property to create the content of the SOAP Body element for an outgoing message.

For more information about how to use the [OutboundBodyLocation](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.OutboundBodyLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>.OutboundBodyLocation') property, see [Specifying the
            Message Body for the WCF Adapters](https://docs.microsoft.com/en-us/biztalk/core/specifying-the-message-body-for-the-wcf-adapters 'https://docs.microsoft.com/en-us/biztalk/core/specifying-the-message-body-for-the-wcf-adapters').

For send port, this property is valid only for solicit-response ports.

It defaults to [Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseBodyElement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseBodyElement 'Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseBodyElement').