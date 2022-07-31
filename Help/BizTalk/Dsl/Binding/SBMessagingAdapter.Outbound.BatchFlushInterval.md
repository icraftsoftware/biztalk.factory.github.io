#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SBMessagingAdapter](SBMessagingAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter').[Outbound](SBMessagingAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound')

## SBMessagingAdapter.Outbound.BatchFlushInterval Property

Specifies a timespan value that indicates the interval when the message batches being sent to a Queue or a Topic
are flushed.

```csharp
public System.TimeSpan BatchFlushInterval { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks

For more information about batching with respect to Service Bus Queues and Topics, see the Client-side batching
section at [Best
            Practices for performance improvements using Service Bus brokered messaging](https://docs.microsoft.com/en-us/azure/service-bus-messaging/service-bus-performance-improvements#client-side-batching 'https://docs.microsoft.com/en-us/azure/service-bus-messaging/service-bus-performance-improvements#client-side-batching').

It defaults to `20` milliseconds.