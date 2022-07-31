#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfBindingCentricAdapterBase&lt;TAddress,TBinding,TConfig&gt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')

## WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.InboundBodyPathExpression Property

Specify the body path expression to identify a specific part of an incoming message used to create the BizTalk
message body part. This body path expression is evaluated against the immediate child element of the SOAP Body node
of an incoming message. If this body path expression returns more than one node, only the first node is chosen for
the BizTalk message body part. This property is required if the [InboundBodyLocation](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.InboundBodyLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.InboundBodyLocation') property is set to
[Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath 'Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath').

```csharp
public string InboundBodyPathExpression { get; set; }
```

Implements [InboundBodyPathExpression](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling.InboundBodyPathExpression 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling.InboundBodyPathExpression')

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

For more information about how to use the [InboundBodyPathExpression](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.InboundBodyPathExpression.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.InboundBodyPathExpression') property, see [WCF Adapters
            Property Schema and Properties](https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters-property-schema-and-properties 'https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters-property-schema-and-properties').

For send port, this property is valid only for solicit-response ports.

It defaults to [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty').