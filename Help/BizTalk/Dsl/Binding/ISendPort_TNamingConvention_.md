#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding')

## ISendPort<TNamingConvention> Interface

```csharp
public interface ISendPort<TNamingConvention> :
Be.Stateless.BizTalk.Dsl.Binding.ISendPort,
Be.Stateless.BizTalk.IFluentInterface,
Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>,
Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution
    where TNamingConvention : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.ISendPort_TNamingConvention_.TNamingConvention'></a>

`TNamingConvention`

Derived  
&#8627; [SendPortBase&lt;TNamingConvention&gt;](SendPortBase_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>')

Implements [ISendPort](ISendPort.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort'), [Be.Stateless.BizTalk.IFluentInterface](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.IFluentInterface 'Be.Stateless.BizTalk.IFluentInterface'), [Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding&lt;](IObjectBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>')[TNamingConvention](ISendPort_TNamingConvention_.md#Be.Stateless.BizTalk.Dsl.Binding.ISendPort_TNamingConvention_.TNamingConvention 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>.TNamingConvention')[&gt;](IObjectBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>'), [ISupportNameResolution](ISupportNameResolution.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution')

| Properties | |
| :--- | :--- |
| [ApplicationBinding](ISendPort_TNamingConvention_.ApplicationBinding.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>.ApplicationBinding') | |
| [BackupTransport](ISendPort_TNamingConvention_.BackupTransport.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>.BackupTransport') | |
| [Filter](ISendPort_TNamingConvention_.Filter.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>.Filter') | Define conditions based on message context's promoted properties that determine which messages are routed to the send port. |
| [OrderedDelivery](ISendPort_TNamingConvention_.OrderedDelivery.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>.OrderedDelivery') | Whether to send messages in order of receipt. |
| [Priority](ISendPort_TNamingConvention_.Priority.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>.Priority') | Priority of the resend attempt. |
| [ReceivePipeline](ISendPort_TNamingConvention_.ReceivePipeline.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>.ReceivePipeline') | |
| [SendPipeline](ISendPort_TNamingConvention_.SendPipeline.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>.SendPipeline') | |
| [State](ISendPort_TNamingConvention_.State.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>.State') | The state of the send port. |
| [StopSendingOnOrderedDeliveryFailure](ISendPort_TNamingConvention_.StopSendingOnOrderedDeliveryFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>.StopSendingOnOrderedDeliveryFailure') | Whether to stop sending subsequent messages that follow a failed message when [OrderedDelivery](ISendPort_TNamingConvention_.OrderedDelivery.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>.OrderedDelivery') option is enabled. |
| [Transport](ISendPort_TNamingConvention_.Transport.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>.Transport') | |
