#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter](WcfNetMsmqAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter').[Outbound](WcfNetMsmqAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Outbound')

## WcfNetMsmqAdapter.Outbound.OutboundXmlTemplate Property

Specify the XML-formatted template for the content of the SOAP Body element of an outgoing response message. This
property is required if the [OutboundBodyLocation](WcfNetMsmqAdapter.Outbound.OutboundBodyLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Outbound.OutboundBodyLocation') property is set to [Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseTemplate](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseTemplate 'Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseTemplate').

```csharp
public string OutboundXmlTemplate { get; set; }
```

Implements [OutboundXmlTemplate](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOutboundMessageMarshalling.OutboundXmlTemplate 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOutboundMessageMarshalling.OutboundXmlTemplate')

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

For more information about how to use the [OutboundXmlTemplate](WcfNetMsmqAdapter.Outbound.OutboundXmlTemplate.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Outbound.OutboundXmlTemplate') property, see [Specifying
            the Message Body for the WCF Adapters](https://docs.microsoft.com/en-us/biztalk/core/specifying-the-message-body-for-the-wcf-adapters 'https://docs.microsoft.com/en-us/biztalk/core/specifying-the-message-body-for-the-wcf-adapters').

For send port, this property is valid only for solicit-response ports.

It defaults to [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty').