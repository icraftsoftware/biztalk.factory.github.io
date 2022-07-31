#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfTwoWayAdapterBase&lt;TAddress,TBinding,TConfig&gt;](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>')

## WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>.InboundNodeEncoding Property

Specify the type of encoding that the WCF-NetTcp send adapter uses to decode for the node identified by the XPath
specified in [InboundBodyPathExpression](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.InboundBodyPathExpression.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>.InboundBodyPathExpression'). This property is required if the [InboundBodyLocation](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.InboundBodyLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>.InboundBodyLocation') property is set to [Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath 'Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath').

```csharp
public Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat InboundNodeEncoding { get; set; }
```

Implements [InboundNodeEncoding](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling.InboundNodeEncoding 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling.InboundNodeEncoding')

#### Property Value
[Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat 'Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat')

### Remarks

- [Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat.Base64](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat.Base64 'Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat.Base64') — Base64 encoding.
- [Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat.Hex](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat.Hex 'Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat.Hex') — Hexadecimal encoding.
- [Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat.String](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat.String 'Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat.String') — UTF-8 Text encoding.
- [Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat.Xml](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat.Xml 'Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat.Xml') — The WCF adapters create the BizTalk message body with the outer XML of
              the node selected by the body path expression in [InboundBodyPathExpression](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.InboundBodyPathExpression.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>.InboundBodyPathExpression').

For send port, this property is valid only for solicit-response ports.

It defaults to [Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat.Xml](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat.Xml 'Microsoft.BizTalk.Adapter.Wcf.Config.MessageBodyFormat.Xml').