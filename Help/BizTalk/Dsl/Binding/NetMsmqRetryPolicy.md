#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration](Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.md 'Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration')

## NetMsmqRetryPolicy Class

```csharp
public class NetMsmqRetryPolicy
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; NetMsmqRetryPolicy

| Properties | |
| :--- | :--- |
| [Default](NetMsmqRetryPolicy.Default.md 'Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.NetMsmqRetryPolicy.Default') | |
| [MaxRetryCycles](NetMsmqRetryPolicy.MaxRetryCycles.md 'Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.NetMsmqRetryPolicy.MaxRetryCycles') | Gets or sets the maximum number of retry cycles to attempt delivery of messages to the receiving application. |
| [ReceiveRetryCount](NetMsmqRetryPolicy.ReceiveRetryCount.md 'Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.NetMsmqRetryPolicy.ReceiveRetryCount') | Gets or sets the maximum number of immediate retries that the queue manager should attempt if transmission of a message from the application queue to the application fails. |
| [RetryCycleDelay](NetMsmqRetryPolicy.RetryCycleDelay.md 'Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.NetMsmqRetryPolicy.RetryCycleDelay') | Gets or sets a value that specifies how long to wait before attempting another retry cycle when attempting to deliver a message that could not be delivered. |
| [TimeToLive](NetMsmqRetryPolicy.TimeToLive.md 'Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.NetMsmqRetryPolicy.TimeToLive') | Gets or sets a value that specifies how long messages are valid. When this time has elapsed, the message is placed in a dead-letter queue (if available). |
