#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter](WcfNetMsmqAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter').[Outbound](WcfNetMsmqAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Outbound')

## WcfNetMsmqAdapter.Outbound.DeadLetterQueue Property

Specify the dead-letter queue where messages that have failed to be delivered to the application will be
transferred.

```csharp
public System.ServiceModel.DeadLetterQueue DeadLetterQueue { get; set; }
```

Implements [DeadLetterQueue](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqBinding.DeadLetterQueue 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqBinding.DeadLetterQueue')

#### Property Value
[System.ServiceModel.DeadLetterQueue](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.DeadLetterQueue 'System.ServiceModel.DeadLetterQueue')

### Remarks

- [System.ServiceModel.DeadLetterQueue.None](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.DeadLetterQueue.None 'System.ServiceModel.DeadLetterQueue.None') — No dead-letter queue is to be used.
- [System.ServiceModel.DeadLetterQueue.System](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.DeadLetterQueue.System 'System.ServiceModel.DeadLetterQueue.System') — Use the system-wide dead-letter queue.
- [System.ServiceModel.DeadLetterQueue.Custom](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.DeadLetterQueue.Custom 'System.ServiceModel.DeadLetterQueue.Custom') — Use a custom dead-letter queue.
            For more information about the messages delivered to the dead-letter queue, see [WCF-NetMsmq
            Transport Properties Dialog Box, Send, Binding Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-netmsmq-transport-properties-dialog-box-send-binding-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-netmsmq-transport-properties-dialog-box-send-binding-tab').

The custom dead-letter queue is supported only in Message Queuing (MSMQ) 4.0, released with Windows Vista.

It defaults to [System.ServiceModel.DeadLetterQueue.System](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.DeadLetterQueue.System 'System.ServiceModel.DeadLetterQueue.System')