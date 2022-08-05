#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter](WcfNetMsmqAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter').[Outbound](WcfNetMsmqAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Outbound')

## WcfNetMsmqAdapter.Outbound.CustomDeadLetterQueue Property

Specify the fully qualified URI with the net.msmq scheme for the location of the per-application dead-letter
queue, where messages that have expired or that have failed transfer or delivery are placed.

```csharp
public string CustomDeadLetterQueue { get; set; }
```

Implements [CustomDeadLetterQueue](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqBinding.CustomDeadLetterQueue 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqBinding.CustomDeadLetterQueue')

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

For example, `net.msmq://localhost/deadLetterQueueName`. The dead-letter queue is a queue on the queue
manager of the sending application for expired messages that have failed to be delivered. This property is
required if the [DeadLetterQueue](WcfNetMsmqAdapter.Outbound.DeadLetterQueue.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Outbound.DeadLetterQueue') property is set to [System.ServiceModel.DeadLetterQueue.Custom](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.DeadLetterQueue.Custom 'System.ServiceModel.DeadLetterQueue.Custom').

It defaults to [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty')