#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig> Class

```csharp
public abstract class WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig> : Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress, TBinding, TConfig>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigEndpointBehavior,
Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling,
Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOutboundMessageMarshalling,
Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts
    where TBinding : System.ServiceModel.Configuration.StandardBindingElement, new()
    where TConfig : Microsoft.BizTalk.Adapter.Wcf.Config.AdapterConfig, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigAddress, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigBinding, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigEndpointBehavior, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigIdentity, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOutboundMessageMarshalling, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.TAddress'></a>

`TAddress`

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.TBinding'></a>

`TBinding`

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.TConfig'></a>

`TConfig`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase&lt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TAddress](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.TAddress 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.TAddress')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TBinding](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.TBinding')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TConfig](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.TConfig 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.TConfig')[&gt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>') &#129106; WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>

Derived  
&#8627; [WcfCustomAdapterBase&lt;TAddress,TBinding,TConfig&gt;](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>')  
&#8627; [WcfLobAdapterBase&lt;TAddress,TBinding,TConfig&gt;](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>')

Implements [IAdapterConfigEndpointBehavior](IAdapterConfigEndpointBehavior.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigEndpointBehavior'), [Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling'), [Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOutboundMessageMarshalling](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOutboundMessageMarshalling 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOutboundMessageMarshalling'), [Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts')

| Constructors | |
| :--- | :--- |
| [WcfBindingCentricAdapterBase(ProtocolType)](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.WcfBindingCentricAdapterBase(ProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.WcfBindingCentricAdapterBase(Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | |

| Properties | |
| :--- | :--- |
| [CloseTimeout](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.CloseTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.CloseTimeout') | Gets or sets the interval of time after which the close method, invoked by a communication object, times out. |
| [EndpointBehaviors](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.EndpointBehaviors.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.EndpointBehaviors') | |
| [InboundBodyLocation](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.InboundBodyLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.InboundBodyLocation') | Specify the data selection for the SOAP Body element of incoming WCF messages. |
| [InboundBodyPathExpression](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.InboundBodyPathExpression.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.InboundBodyPathExpression') | Specify the body path expression to identify a specific part of an incoming message used to create the BizTalk message body part. This body path expression is evaluated against the immediate child element of the SOAP Body node of an incoming message. If this body path expression returns more than one node, only the first node is chosen for the BizTalk message body part. This property is required if the [InboundBodyLocation](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.InboundBodyLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.InboundBodyLocation') property is set to [Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath 'Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath'). |
| [InboundNodeEncoding](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.InboundNodeEncoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.InboundNodeEncoding') | Specify the type of encoding that the WCF-NetTcp send adapter uses to decode for the node identified by the XPath specified in [InboundBodyPathExpression](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.InboundBodyPathExpression.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.InboundBodyPathExpression'). This property is required if the [InboundBodyLocation](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.InboundBodyLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.InboundBodyLocation') property is set to [Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath 'Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath'). |
| [OpenTimeout](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.OpenTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.OpenTimeout') | Gets or sets the interval of time after which the open method, invoked by a communication object, times out. |
| [OutboundBodyLocation](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.OutboundBodyLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.OutboundBodyLocation') | Specify the data selection for the SOAP Body element of outgoing WCF messages. |
| [OutboundXmlTemplate](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.OutboundXmlTemplate.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.OutboundXmlTemplate') | Specify the XML-formatted template for the content of the SOAP Body element of an outgoing response message. This property is required if the [OutboundBodyLocation](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.OutboundBodyLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.OutboundBodyLocation') property is set to [Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseTemplate](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseTemplate 'Microsoft.BizTalk.Adapter.Wcf.Config.OutboundMessageBodySelection.UseTemplate'). |
| [SendTimeout](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.SendTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.SendTimeout') | Gets or sets the interval of time after which the send method, invoked by a communication object, times out. |

| Methods | |
| :--- | :--- |
| [Save(IPropertyBag)](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | |
