#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter](WcfNetMsmqAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter').[Inbound](WcfNetMsmqAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound')

## WcfNetMsmqAdapter.Inbound.InboundBodyLocation Property

Specify the data selection for the SOAP Body element of incoming WCF messages.

```csharp
public Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection InboundBodyLocation { get; set; }
```

Implements [InboundBodyLocation](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling.InboundBodyLocation 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling.InboundBodyLocation')

#### Property Value
[Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection 'Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection')

### Remarks

- [Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyElement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyElement 'Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyElement') — Use the content of the SOAP Body element of an
              incoming message to create the BizTalk message body part. If the Body element has more than one child element,
              only the first element becomes the BizTalk message body part.
- [Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath 'Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath') — Use the body path expression in the [InboundBodyPathExpression](WcfNetMsmqAdapter.Inbound.InboundBodyPathExpression.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound.InboundBodyPathExpression') property to create the BizTalk message body part. The body path expression is
              evaluated against the immediate child element of the SOAP Body element of an incoming message. This property is
              valid only for solicit-response ports.
- [Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseEnvelope](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseEnvelope 'Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseEnvelope') — Create the BizTalk message body part from the entire
              SOAP Envelope of an incoming message.

For more information about how to use the [InboundBodyLocation](WcfNetMsmqAdapter.Inbound.InboundBodyLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound.InboundBodyLocation') property, see [Specifying
            the Message Body for the WCF Adapters](https://docs.microsoft.com/en-us/biztalk/core/specifying-the-message-body-for-the-wcf-adapters 'https://docs.microsoft.com/en-us/biztalk/core/specifying-the-message-body-for-the-wcf-adapters').

It defaults to [Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyElement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyElement 'Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyElement').