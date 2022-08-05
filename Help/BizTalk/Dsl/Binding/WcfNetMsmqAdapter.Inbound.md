#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter](WcfNetMsmqAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter')

## WcfNetMsmqAdapter.Inbound Class

The WCF-NetMsmq adapter provides disconnected cross-computer communication by using queuing technology in an
environment where both the services and clients are WCF based. It uses the Message Queuing (MSMQ) transport, and
messages have binary encoding.

```csharp
public class WcfNetMsmqAdapter.Inbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<Microsoft.BizTalk.Adapter.Wcf.Config.NetMsmqRLConfig>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation,
Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundDisableLocationOnFailure,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundSuspendRequestMessageOnFailure,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxConcurrentCalls,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxReceivedMessageSize,
Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOrdering
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase&lt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.EndpointAddress](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.EndpointAddress 'System.ServiceModel.EndpointAddress')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.Configuration.NetMsmqBindingElement](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Configuration.NetMsmqBindingElement 'System.ServiceModel.Configuration.NetMsmqBindingElement')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.NetMsmqRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.NetMsmqRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.NetMsmqRLConfig')[&gt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase&lt;](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.EndpointAddress](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.EndpointAddress 'System.ServiceModel.EndpointAddress')[,](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.Configuration.NetMsmqBindingElement](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Configuration.NetMsmqBindingElement 'System.ServiceModel.Configuration.NetMsmqBindingElement')[,](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.NetMsmqRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.NetMsmqRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.NetMsmqRLConfig')[&gt;](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter&lt;](WcfNetMsmqAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.NetMsmqRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.NetMsmqRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.NetMsmqRLConfig')[&gt;](WcfNetMsmqAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>') &#129106; Inbound

Implements [IInboundAdapter](IInboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation'), [Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling'), [IAdapterConfigInboundDisableLocationOnFailure](IAdapterConfigInboundDisableLocationOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundDisableLocationOnFailure'), [IAdapterConfigInboundSuspendRequestMessageOnFailure](IAdapterConfigInboundSuspendRequestMessageOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundSuspendRequestMessageOnFailure'), [IAdapterConfigMaxConcurrentCalls](IAdapterConfigMaxConcurrentCalls.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxConcurrentCalls'), [IAdapterConfigMaxReceivedMessageSize](IAdapterConfigMaxReceivedMessageSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxReceivedMessageSize'), [Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOrdering](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOrdering 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOrdering')

### See Also
- [What Is the WCF-NetMsmq Adapter?](https://docs.microsoft.com/en-us/biztalk/core/what-is-the-wcf-netmsmq-adapter 'https://docs.microsoft.com/en-us/biztalk/core/what-is-the-wcf-netmsmq-adapter')
- [How to Configure a WCF-NetMsmq Receive Location](https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-a-wcf-netmsmq-receive-location 'https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-a-wcf-netmsmq-receive-location')
- [WCF-NetMsmq Transport Properties Dialog Box, Receive, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-netmsmq-transport-properties-dialog-box-receive-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-netmsmq-transport-properties-dialog-box-receive-security-tab')
- [WCF
            Adapters Property Schema and Properties](https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters-property-schema-and-properties 'https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters-property-schema-and-properties')

| Constructors | |
| :--- | :--- |
| [Inbound()](WcfNetMsmqAdapter.Inbound.Inbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound.Inbound()') | |
| [Inbound(Action&lt;Inbound&gt;)](WcfNetMsmqAdapter.Inbound.Inbound(Action_Inbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound.Inbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound>)') | |

| Properties | |
| :--- | :--- |
| [DisableLocationOnFailure](WcfNetMsmqAdapter.Inbound.DisableLocationOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound.DisableLocationOnFailure') | |
| [InboundBodyLocation](WcfNetMsmqAdapter.Inbound.InboundBodyLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound.InboundBodyLocation') | Specify the data selection for the SOAP Body element of incoming WCF messages. |
| [InboundBodyPathExpression](WcfNetMsmqAdapter.Inbound.InboundBodyPathExpression.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound.InboundBodyPathExpression') | Specify the body path expression to identify a specific part of an incoming message used to create the BizTalk message body part. This body path expression is evaluated against the immediate child element of the SOAP Body node of an incoming message. If this body path expression returns more than one node, only the first node is chosen for the BizTalk message body part. This property is required if the [InboundBodyLocation](WcfNetMsmqAdapter.Inbound.InboundBodyLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound.InboundBodyLocation') property is set to [Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath 'Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath'). |
| [InboundNodeEncoding](WcfNetMsmqAdapter.Inbound.InboundNodeEncoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound.InboundNodeEncoding') | Specify the type of encoding that the WCF-NetTcp send adapter uses to decode for the node identified by the XPath specified in [InboundBodyPathExpression](WcfNetMsmqAdapter.Inbound.InboundBodyPathExpression.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound.InboundBodyPathExpression'). This property is required if the [InboundBodyLocation](WcfNetMsmqAdapter.Inbound.InboundBodyLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound.InboundBodyLocation') property is set to [Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath 'Microsoft.BizTalk.Adapter.Wcf.Config.InboundMessageBodySelection.UseBodyPath'). |
| [MaxConcurrentCalls](WcfNetMsmqAdapter.Inbound.MaxConcurrentCalls.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound.MaxConcurrentCalls') | |
| [MaxReceivedMessageSize](WcfNetMsmqAdapter.Inbound.MaxReceivedMessageSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound.MaxReceivedMessageSize') | |
| [OrderedProcessing](WcfNetMsmqAdapter.Inbound.OrderedProcessing.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound.OrderedProcessing') | Specify whether to process messages serially. |
| [SuspendRequestMessageOnFailure](WcfNetMsmqAdapter.Inbound.SuspendRequestMessageOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound.SuspendRequestMessageOnFailure') | |