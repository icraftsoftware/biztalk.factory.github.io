#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding')

## ReceiveLocationBase<TNamingConvention> Class

```csharp
public abstract class ReceiveLocationBase<TNamingConvention> :
Be.Stateless.BizTalk.Dsl.Binding.IReceiveLocation<TNamingConvention>,
Be.Stateless.BizTalk.Dsl.Binding.IReceiveLocation,
Be.Stateless.BizTalk.IFluentInterface,
Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>,
Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution,
Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride,
Be.Stateless.BizTalk.Dsl.ISupportValidation,
Be.Stateless.BizTalk.Dsl.IVisitable<Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor>
    where TNamingConvention : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase_TNamingConvention_.TNamingConvention'></a>

`TNamingConvention`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ReceiveLocationBase<TNamingConvention>

Derived  
&#8627; [ReceiveLocation](ReceiveLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocation')

Implements [Be.Stateless.BizTalk.Dsl.Binding.IReceiveLocation&lt;](IReceiveLocation_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IReceiveLocation<TNamingConvention>')[TNamingConvention](ReceiveLocationBase_TNamingConvention_.md#Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase_TNamingConvention_.TNamingConvention 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.TNamingConvention')[&gt;](IReceiveLocation_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IReceiveLocation<TNamingConvention>'), [IReceiveLocation](IReceiveLocation.md 'Be.Stateless.BizTalk.Dsl.Binding.IReceiveLocation'), [Be.Stateless.BizTalk.IFluentInterface](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.IFluentInterface 'Be.Stateless.BizTalk.IFluentInterface'), [Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding&lt;](IObjectBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>')[TNamingConvention](ReceiveLocationBase_TNamingConvention_.md#Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase_TNamingConvention_.TNamingConvention 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.TNamingConvention')[&gt;](IObjectBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>'), [ISupportNameResolution](ISupportNameResolution.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution'), [ISupportEnvironmentOverride](ISupportEnvironmentOverride.md 'Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation'), [Be.Stateless.BizTalk.Dsl.IVisitable&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.IVisitable-1 'Be.Stateless.BizTalk.Dsl.IVisitable`1')[IApplicationBindingVisitor](IApplicationBindingVisitor.md 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.IVisitable-1 'Be.Stateless.BizTalk.Dsl.IVisitable`1')

| Constructors | |
| :--- | :--- |
| [ReceiveLocationBase()](ReceiveLocationBase_TNamingConvention_.ReceiveLocationBase().md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.ReceiveLocationBase()') | |
| [ReceiveLocationBase(Action&lt;IReceiveLocation&lt;TNamingConvention&gt;&gt;)](ReceiveLocationBase_TNamingConvention_.ReceiveLocationBase(Action_IReceiveLocation_TNamingConvention__).md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.ReceiveLocationBase(System.Action<Be.Stateless.BizTalk.Dsl.Binding.IReceiveLocation<TNamingConvention>>)') | |

| Properties | |
| :--- | :--- |
| [Description](ReceiveLocationBase_TNamingConvention_.Description.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.Description') | |
| [Enabled](ReceiveLocationBase_TNamingConvention_.Enabled.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.Enabled') | |
| [Name](ReceiveLocationBase_TNamingConvention_.Name.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.Name') | |
| [ReceivePipeline](ReceiveLocationBase_TNamingConvention_.ReceivePipeline.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.ReceivePipeline') | |
| [ReceivePort](ReceiveLocationBase_TNamingConvention_.ReceivePort.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.ReceivePort') | |
| [SendPipeline](ReceiveLocationBase_TNamingConvention_.SendPipeline.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.SendPipeline') | |
| [Transport](ReceiveLocationBase_TNamingConvention_.Transport.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.Transport') | |

| Methods | |
| :--- | :--- |
| [ApplyEnvironmentOverrides(string)](ReceiveLocationBase_TNamingConvention_.ApplyEnvironmentOverrides(string).md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.ApplyEnvironmentOverrides(string)') | |
| [ResolveName()](ReceiveLocationBase_TNamingConvention_.ResolveName().md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.ResolveName()') | |

| Explicit Interface Implementations | |
| :--- | :--- |
| [Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string)](ReceiveLocationBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string).md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string)') | |
| [Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate()](ReceiveLocationBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate()') | |
| [Be.Stateless.BizTalk.Dsl.IVisitable&lt;Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor&gt;.Accept&lt;TVisitor&gt;(TVisitor)](ReceiveLocationBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.IVisitable_Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor_.Accept_TVisitor_(TVisitor).md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.IVisitable<Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor>.Accept<TVisitor>(TVisitor)') | |
| [Be.Stateless.BizTalk.IFluentInterface.GetType()](ReceiveLocationBase_TNamingConvention_.Be.Stateless.BizTalk.IFluentInterface.GetType().md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>.Be.Stateless.BizTalk.IFluentInterface.GetType()') | |
