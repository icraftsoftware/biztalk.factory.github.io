#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter](WcfNetMsmqAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter').[Outbound](WcfNetMsmqAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Outbound')

## WcfNetMsmqAdapter.Outbound.OutboundBodyLocation Property

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
- [Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseTemplate](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseTemplate 'Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseTemplate') — Use the template supplied in the [OutboundXmlTemplate](WcfNetMsmqAdapter.Outbound.OutboundXmlTemplate.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Outbound.OutboundXmlTemplate') property to create the content of the SOAP Body element for an outgoing message.

For more information about how to use the [OutboundBodyLocation](WcfNetMsmqAdapter.Outbound.OutboundBodyLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Outbound.OutboundBodyLocation') property, see [Specifying
            the Message Body for the WCF Adapters](https://docs.microsoft.com/en-us/biztalk/core/specifying-the-message-body-for-the-wcf-adapters 'https://docs.microsoft.com/en-us/biztalk/core/specifying-the-message-body-for-the-wcf-adapters').

For send port, this property is valid only for solicit-response ports.

It defaults to [Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseBodyElement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseBodyElement 'Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseBodyElement').