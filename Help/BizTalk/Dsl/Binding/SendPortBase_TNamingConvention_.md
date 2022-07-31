#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding')

## SendPortBase<TNamingConvention> Class

```csharp
public abstract class SendPortBase<TNamingConvention> :
Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>,
Be.Stateless.BizTalk.Dsl.Binding.ISendPort,
Be.Stateless.BizTalk.IFluentInterface,
Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>,
Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution,
Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride,
Be.Stateless.BizTalk.Dsl.ISupportValidation,
Be.Stateless.BizTalk.Dsl.IVisitable<Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor>
    where TNamingConvention : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.SendPortBase_TNamingConvention_.TNamingConvention'></a>

`TNamingConvention`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; SendPortBase<TNamingConvention>

Derived  
&#8627; [SendPort](SendPort.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPort')

Implements [Be.Stateless.BizTalk.Dsl.Binding.ISendPort&lt;](ISendPort_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>')[TNamingConvention](SendPortBase_TNamingConvention_.md#Be.Stateless.BizTalk.Dsl.Binding.SendPortBase_TNamingConvention_.TNamingConvention 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.TNamingConvention')[&gt;](ISendPort_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>'), [ISendPort](ISendPort.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort'), [Be.Stateless.BizTalk.IFluentInterface](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.IFluentInterface 'Be.Stateless.BizTalk.IFluentInterface'), [Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding&lt;](IObjectBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>')[TNamingConvention](SendPortBase_TNamingConvention_.md#Be.Stateless.BizTalk.Dsl.Binding.SendPortBase_TNamingConvention_.TNamingConvention 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.TNamingConvention')[&gt;](IObjectBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>'), [ISupportNameResolution](ISupportNameResolution.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution'), [ISupportEnvironmentOverride](ISupportEnvironmentOverride.md 'Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation'), [Be.Stateless.BizTalk.Dsl.IVisitable&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.IVisitable-1 'Be.Stateless.BizTalk.Dsl.IVisitable`1')[IApplicationBindingVisitor](IApplicationBindingVisitor.md 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.IVisitable-1 'Be.Stateless.BizTalk.Dsl.IVisitable`1')

| Constructors | |
| :--- | :--- |
| [SendPortBase()](SendPortBase_TNamingConvention_.SendPortBase().md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.SendPortBase()') | |
| [SendPortBase(Action&lt;ISendPort&lt;TNamingConvention&gt;&gt;)](SendPortBase_TNamingConvention_.SendPortBase(Action_ISendPort_TNamingConvention__).md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.SendPortBase(System.Action<Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>>)') | |

| Properties | |
| :--- | :--- |
| [ApplicationBinding](SendPortBase_TNamingConvention_.ApplicationBinding.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.ApplicationBinding') | |
| [BackupTransport](SendPortBase_TNamingConvention_.BackupTransport.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.BackupTransport') | |
| [Description](SendPortBase_TNamingConvention_.Description.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.Description') | |
| [Filter](SendPortBase_TNamingConvention_.Filter.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.Filter') | |
| [IsTwoWay](SendPortBase_TNamingConvention_.IsTwoWay.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.IsTwoWay') | |
| [Name](SendPortBase_TNamingConvention_.Name.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.Name') | |
| [OrderedDelivery](SendPortBase_TNamingConvention_.OrderedDelivery.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.OrderedDelivery') | |
| [Priority](SendPortBase_TNamingConvention_.Priority.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.Priority') | |
| [ReceivePipeline](SendPortBase_TNamingConvention_.ReceivePipeline.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.ReceivePipeline') | |
| [SendPipeline](SendPortBase_TNamingConvention_.SendPipeline.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.SendPipeline') | |
| [State](SendPortBase_TNamingConvention_.State.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.State') | |
| [StopSendingOnOrderedDeliveryFailure](SendPortBase_TNamingConvention_.StopSendingOnOrderedDeliveryFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.StopSendingOnOrderedDeliveryFailure') | |
| [Transport](SendPortBase_TNamingConvention_.Transport.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.Transport') | |

| Methods | |
| :--- | :--- |
| [ApplyEnvironmentOverrides(string)](SendPortBase_TNamingConvention_.ApplyEnvironmentOverrides(string).md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.ApplyEnvironmentOverrides(string)') | |
| [ResolveName()](SendPortBase_TNamingConvention_.ResolveName().md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.ResolveName()') | |

| Explicit Interface Implementations | |
| :--- | :--- |
| [Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string)](SendPortBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string).md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string)') | |
| [Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate()](SendPortBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate()') | |
| [Be.Stateless.BizTalk.Dsl.IVisitable&lt;Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor&gt;.Accept&lt;TVisitor&gt;(TVisitor)](SendPortBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.IVisitable_Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor_.Accept_TVisitor_(TVisitor).md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.IVisitable<Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor>.Accept<TVisitor>(TVisitor)') | |
| [Be.Stateless.BizTalk.IFluentInterface.GetType()](SendPortBase_TNamingConvention_.Be.Stateless.BizTalk.IFluentInterface.GetType().md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortBase<TNamingConvention>.Be.Stateless.BizTalk.IFluentInterface.GetType()') | |
