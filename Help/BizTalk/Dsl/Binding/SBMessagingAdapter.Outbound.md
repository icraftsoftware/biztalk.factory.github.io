#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SBMessagingAdapter](SBMessagingAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter')

## SBMessagingAdapter.Outbound Class

The SB-Messaging adapter allows to send and receive messages from Service Bus entities like Queues, Topics, and
Relays. You can use the SB-Messaging adapters to bridge the connectivity between Windows Azure and on-premises
BizTalk Server, thereby enabling users to create a typical hybrid application.

```csharp
public class SBMessagingAdapter.Outbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<Microsoft.BizTalk.Adapter.SBMessaging.SBMessagingTLConfig>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IOutboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter&lt;](SBMessagingAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>')[Microsoft.BizTalk.Adapter.SBMessaging.SBMessagingTLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.SBMessaging.SBMessagingTLConfig 'Microsoft.BizTalk.Adapter.SBMessaging.SBMessagingTLConfig')[&gt;](SBMessagingAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>') &#129106; Outbound

Implements [IOutboundAdapter](IOutboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IOutboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation')

### See Also
- [SB-Messaging Adapter](https://docs.microsoft.com/en-us/biztalk/core/sb-messaging-adapter 'https://docs.microsoft.com/en-us/biztalk/core/sb-messaging-adapter')

| Constructors | |
| :--- | :--- |
| [Outbound()](SBMessagingAdapter.Outbound.Outbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.Outbound()') | |
| [Outbound(Action&lt;Outbound&gt;)](SBMessagingAdapter.Outbound.Outbound(Action_Outbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.Outbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound>)') | |

| Properties | |
| :--- | :--- |
| [BatchFlushInterval](SBMessagingAdapter.Outbound.BatchFlushInterval.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.BatchFlushInterval') | Specifies a timespan value that indicates the interval when the message batches being sent to a Queue or a Topic are flushed. |
| [CustomBrokeredPropertyNamespace](SBMessagingAdapter.Outbound.CustomBrokeredPropertyNamespace.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.CustomBrokeredPropertyNamespace') | Specify the namespace that contains the BizTalk message context properties that you want to write as user-defined Brokered Message properties on the outgoing message sent to the Service Bus Queue. |
| [DefaultCorrelationId](SBMessagingAdapter.Outbound.DefaultCorrelationId.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.DefaultCorrelationId') | Specify the identifier of the correlation. |
| [DefaultLabel](SBMessagingAdapter.Outbound.DefaultLabel.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.DefaultLabel') | Specify the application specific label. |
| [DefaultMessageId](SBMessagingAdapter.Outbound.DefaultMessageId.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.DefaultMessageId') | Specify the identifier of the message. |
| [DefaultPartitionKey](SBMessagingAdapter.Outbound.DefaultPartitionKey.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.DefaultPartitionKey') | Gets or sets a partition key for sending a transactional message to a queue or topic that is not session-aware. |
| [DefaultReplyTo](SBMessagingAdapter.Outbound.DefaultReplyTo.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.DefaultReplyTo') | Specify the default address of the queue to reply to. |
| [DefaultReplyToSessionId](SBMessagingAdapter.Outbound.DefaultReplyToSessionId.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.DefaultReplyToSessionId') | Specify the address of the queue to reply to. |
| [DefaultScheduledEnqueueTimeUtc](SBMessagingAdapter.Outbound.DefaultScheduledEnqueueTimeUtc.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.DefaultScheduledEnqueueTimeUtc') | Specify the date and time in UTC at which the message will be enqueued. |
| [DefaultSessionId](SBMessagingAdapter.Outbound.DefaultSessionId.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.DefaultSessionId') | Specify the identifier of the session. |
| [DefaultTimeToLive](SBMessagingAdapter.Outbound.DefaultTimeToLive.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.DefaultTimeToLive') | Specify the message's time to live value. |
| [MaxReceivedMessageSize](SBMessagingAdapter.Outbound.MaxReceivedMessageSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.MaxReceivedMessageSize') | Specifies the maximum size, in bytes, for a message that can be processed by the Azure Service Bus binding. |
| [SendTimeout](SBMessagingAdapter.Outbound.SendTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.SendTimeout') | Specifies a timespan value that indicates the time for a send operation to complete. |
| [SessionIdleTimeout](SBMessagingAdapter.Outbound.SessionIdleTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound.SessionIdleTimeout') | Specifies the timespan value that indicates the period of inactivity that the session waits before timing out. |
