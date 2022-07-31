#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SBMessagingAdapter](SBMessagingAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter').[Outbound](SBMessagingAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound')

## SBMessagingAdapter.Outbound.DefaultTimeToLive Property

Specify the message's time to live value.

```csharp
public System.TimeSpan DefaultTimeToLive { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks

This is the duration after which the message expires, starting from when the message is sent to the Service Bus.

Messages older than their [SBMessaging.TimeToLive](https://docs.microsoft.com/en-us/dotnet/api/SBMessaging.TimeToLive 'SBMessaging.TimeToLive') value will expire and no longer be retained in the message
store. Subscribers will be unable to receive expired messages.

[SBMessaging.TimeToLive](https://docs.microsoft.com/en-us/dotnet/api/SBMessaging.TimeToLive 'SBMessaging.TimeToLive') is the maximum lifetime that a message can receive, but its value cannot exceed the
            specified [Microsoft.ServiceBus.Messaging.QueueDescription.DefaultMessageTimeToLive](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.Messaging.QueueDescription.DefaultMessageTimeToLive 'Microsoft.ServiceBus.Messaging.QueueDescription.DefaultMessageTimeToLive') value on the destination queue or subscription.
            If a lower [SBMessaging.TimeToLive](https://docs.microsoft.com/en-us/dotnet/api/SBMessaging.TimeToLive 'SBMessaging.TimeToLive') value is specified, it will be applied to the individual message. However, a
            larger value specified on the message will be overridden by the entity's [Microsoft.ServiceBus.Messaging.QueueDescription.DefaultMessageTimeToLive](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.Messaging.QueueDescription.DefaultMessageTimeToLive 'Microsoft.ServiceBus.Messaging.QueueDescription.DefaultMessageTimeToLive') value.

It defaults to [System.TimeSpan.MaxValue](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan.MaxValue 'System.TimeSpan.MaxValue').

### See Also
- [BrokeredMessage Properties](https://docs.microsoft.com/en-us/dotnet/api/microsoft.servicebus.messaging.brokeredmessage#properties 'https://docs.microsoft.com/en-us/dotnet/api/microsoft.servicebus.messaging.brokeredmessage#properties')