#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SBMessagingAdapter](SBMessagingAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter').[Inbound](SBMessagingAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Inbound')

## SBMessagingAdapter.Inbound.PrefetchCount Property

Specifies the number of messages that are received simultaneously from the Service Bus Queue or a topic.

```csharp
public int PrefetchCount { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks

Prefetching enables the queue or subscription client to load additional messages from the service when it performs
a receive operation. The client stores these messages in a local cache. The size of the cache is determined by the
value for the Prefetch Count property you specify here.

For more information, refer to the section "Prefetching" at [Best Practices for performance
            improvements using Service Bus Messaging](https://docs.microsoft.com/en-us/azure/service-bus-messaging/service-bus-performance-improvements#prefetching 'https://docs.microsoft.com/en-us/azure/service-bus-messaging/service-bus-performance-improvements#prefetching').

It defaults to `-1`.