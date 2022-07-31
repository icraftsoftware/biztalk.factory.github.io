#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter](WcfNetMsmqAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter').[Outbound](WcfNetMsmqAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Outbound')

## WcfNetMsmqAdapter.Outbound.TimeToLive Property

Specify a time span for how long the messages are valid before they are expired and put into the dead-letter
queue.

```csharp
public System.TimeSpan TimeToLive { get; set; }
```

Implements [TimeToLive](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqBinding.TimeToLive 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqBinding.TimeToLive')

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks

This property is set to ensure that time-sensitive messages do not become stale before they are processed by this
send port. A message in a queue that is not consumed by this send port within the time interval specified is said
to be expired. Expired messages are sent to special queue called the dead-letter queue. The location of the
dead-letter queue is set with the [DeadLetterQueue](WcfNetMsmqAdapter.Outbound.DeadLetterQueue.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Outbound.DeadLetterQueue') property.

It defaults to 1 day.