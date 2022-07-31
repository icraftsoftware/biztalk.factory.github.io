#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SBMessagingAdapter](SBMessagingAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter')

## SBMessagingAdapter.Inbound Class

The SB-Messaging adapter allows to send and receive messages from Service Bus entities like Queues, Topics, and
Relays. You can use the SB-Messaging adapters to bridge the connectivity between Windows Azure and on-premises
BizTalk Server, thereby enabling users to create a typical hybrid application.

```csharp
public class SBMessagingAdapter.Inbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<Microsoft.BizTalk.Adapter.SBMessaging.SBMessagingRLConfig>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter&lt;](SBMessagingAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>')[Microsoft.BizTalk.Adapter.SBMessaging.SBMessagingRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.SBMessaging.SBMessagingRLConfig 'Microsoft.BizTalk.Adapter.SBMessaging.SBMessagingRLConfig')[&gt;](SBMessagingAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>') &#129106; Inbound

Implements [IInboundAdapter](IInboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation')

### See Also
- [SB-Messaging Adapter](https://docs.microsoft.com/en-us/biztalk/core/sb-messaging-adapter 'https://docs.microsoft.com/en-us/biztalk/core/sb-messaging-adapter')

| Constructors | |
| :--- | :--- |
| [Inbound()](SBMessagingAdapter.Inbound.Inbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Inbound.Inbound()') | |
| [Inbound(Action&lt;Inbound&gt;)](SBMessagingAdapter.Inbound.Inbound(Action_Inbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Inbound.Inbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Inbound>)') | |

| Properties | |
| :--- | :--- |
| [CustomBrokeredPropertyNamespace](SBMessagingAdapter.Inbound.CustomBrokeredPropertyNamespace.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Inbound.CustomBrokeredPropertyNamespace') | Specify the namespace that the adapter uses to write the brokered message properties as message context properties on the message received by BizTalk Server. |
| [IsSessionful](SBMessagingAdapter.Inbound.IsSessionful.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Inbound.IsSessionful') | Whether to use a Service Bus session to receive messages from a queue or a subscription. |
| [MaxReceivedMessageSize](SBMessagingAdapter.Inbound.MaxReceivedMessageSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Inbound.MaxReceivedMessageSize') | Specifies the maximum size, in bytes, for a message that can be processed by the Azure Service Bus binding. |
| [OrderedProcessing](SBMessagingAdapter.Inbound.OrderedProcessing.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Inbound.OrderedProcessing') | Whether to preserve message ordering within each session when processing messages. |
| [PrefetchCount](SBMessagingAdapter.Inbound.PrefetchCount.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Inbound.PrefetchCount') | Specifies the number of messages that are received simultaneously from the Service Bus Queue or a topic. |
| [PromoteCustomProperties](SBMessagingAdapter.Inbound.PromoteCustomProperties.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Inbound.PromoteCustomProperties') | Specify whether to promote the brokered message properties. |
| [ReceiveTimeout](SBMessagingAdapter.Inbound.ReceiveTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Inbound.ReceiveTimeout') | Specifies a timespan value that indicates the time for a receive operation to complete. |
| [SessionIdleTimeout](SBMessagingAdapter.Inbound.SessionIdleTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Inbound.SessionIdleTimeout') | Specifies the timespan value that indicates the period of inactivity that the session waits before timing out. |
