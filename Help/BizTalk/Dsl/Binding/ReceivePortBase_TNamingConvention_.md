#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding')

## ReceivePortBase<TNamingConvention> Class

```csharp
public abstract class ReceivePortBase<TNamingConvention> :
Be.Stateless.BizTalk.Dsl.Binding.IReceivePort<TNamingConvention>,
Be.Stateless.BizTalk.Dsl.Binding.IReceivePort,
Be.Stateless.BizTalk.IFluentInterface,
Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>,
Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution,
Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride,
Be.Stateless.BizTalk.Dsl.ISupportValidation,
Be.Stateless.BizTalk.Dsl.IVisitable<Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor>
    where TNamingConvention : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase_TNamingConvention_.TNamingConvention'></a>

`TNamingConvention`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ReceivePortBase<TNamingConvention>

Derived  
&#8627; [ReceivePort](ReceivePort.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePort')

Implements [Be.Stateless.BizTalk.Dsl.Binding.IReceivePort&lt;](IReceivePort_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IReceivePort<TNamingConvention>')[TNamingConvention](ReceivePortBase_TNamingConvention_.md#Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase_TNamingConvention_.TNamingConvention 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>.TNamingConvention')[&gt;](IReceivePort_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IReceivePort<TNamingConvention>'), [IReceivePort](IReceivePort.md 'Be.Stateless.BizTalk.Dsl.Binding.IReceivePort'), [Be.Stateless.BizTalk.IFluentInterface](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.IFluentInterface 'Be.Stateless.BizTalk.IFluentInterface'), [Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding&lt;](IObjectBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>')[TNamingConvention](ReceivePortBase_TNamingConvention_.md#Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase_TNamingConvention_.TNamingConvention 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>.TNamingConvention')[&gt;](IObjectBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>'), [ISupportNameResolution](ISupportNameResolution.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution'), [ISupportEnvironmentOverride](ISupportEnvironmentOverride.md 'Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation'), [Be.Stateless.BizTalk.Dsl.IVisitable&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.IVisitable-1 'Be.Stateless.BizTalk.Dsl.IVisitable`1')[IApplicationBindingVisitor](IApplicationBindingVisitor.md 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.IVisitable-1 'Be.Stateless.BizTalk.Dsl.IVisitable`1')

| Constructors | |
| :--- | :--- |
| [ReceivePortBase()](ReceivePortBase_TNamingConvention_.ReceivePortBase().md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>.ReceivePortBase()') | |
| [ReceivePortBase(Action&lt;IReceivePort&lt;TNamingConvention&gt;&gt;)](ReceivePortBase_TNamingConvention_.ReceivePortBase(Action_IReceivePort_TNamingConvention__).md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>.ReceivePortBase(System.Action<Be.Stateless.BizTalk.Dsl.Binding.IReceivePort<TNamingConvention>>)') | |

| Properties | |
| :--- | :--- |
| [ApplicationBinding](ReceivePortBase_TNamingConvention_.ApplicationBinding.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>.ApplicationBinding') | |
| [Description](ReceivePortBase_TNamingConvention_.Description.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>.Description') | |
| [IsTwoWay](ReceivePortBase_TNamingConvention_.IsTwoWay.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>.IsTwoWay') | |
| [Name](ReceivePortBase_TNamingConvention_.Name.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>.Name') | |
| [ReceiveLocations](ReceivePortBase_TNamingConvention_.ReceiveLocations.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>.ReceiveLocations') | |

| Methods | |
| :--- | :--- |
| [ApplyEnvironmentOverrides(string)](ReceivePortBase_TNamingConvention_.ApplyEnvironmentOverrides(string).md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>.ApplyEnvironmentOverrides(string)') | |
| [ResolveName()](ReceivePortBase_TNamingConvention_.ResolveName().md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>.ResolveName()') | |

| Explicit Interface Implementations | |
| :--- | :--- |
| [Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string)](ReceivePortBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string).md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string)') | |
| [Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate()](ReceivePortBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate()') | |
| [Be.Stateless.BizTalk.Dsl.IVisitable&lt;Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor&gt;.Accept&lt;TVisitor&gt;(TVisitor)](ReceivePortBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.IVisitable_Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor_.Accept_TVisitor_(TVisitor).md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.IVisitable<Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor>.Accept<TVisitor>(TVisitor)') | |
| [Be.Stateless.BizTalk.IFluentInterface.GetType()](ReceivePortBase_TNamingConvention_.Be.Stateless.BizTalk.IFluentInterface.GetType().md 'Be.Stateless.BizTalk.Dsl.Binding.ReceivePortBase<TNamingConvention>.Be.Stateless.BizTalk.IFluentInterface.GetType()') | |
