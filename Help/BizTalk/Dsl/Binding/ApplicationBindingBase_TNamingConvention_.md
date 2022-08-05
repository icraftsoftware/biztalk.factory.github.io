#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding')

## ApplicationBindingBase<TNamingConvention> Class

```csharp
public abstract class ApplicationBindingBase<TNamingConvention> :
Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding<TNamingConvention>,
Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding,
Be.Stateless.BizTalk.IFluentInterface,
Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>,
Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution,
Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingArtifactLookup,
Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride,
Be.Stateless.BizTalk.Dsl.ISupportValidation,
Be.Stateless.BizTalk.Dsl.IVisitable<Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor>
    where TNamingConvention : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase_TNamingConvention_.TNamingConvention'></a>

`TNamingConvention`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ApplicationBindingBase<TNamingConvention>

Derived  
&#8627; [ApplicationBinding](ApplicationBinding.md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding')

Implements [Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding&lt;](IApplicationBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding<TNamingConvention>')[TNamingConvention](ApplicationBindingBase_TNamingConvention_.md#Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase_TNamingConvention_.TNamingConvention 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.TNamingConvention')[&gt;](IApplicationBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding<TNamingConvention>'), [IApplicationBinding](IApplicationBinding.md 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding'), [Be.Stateless.BizTalk.IFluentInterface](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.IFluentInterface 'Be.Stateless.BizTalk.IFluentInterface'), [Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding&lt;](IObjectBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>')[TNamingConvention](ApplicationBindingBase_TNamingConvention_.md#Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase_TNamingConvention_.TNamingConvention 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.TNamingConvention')[&gt;](IObjectBinding_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.IObjectBinding<TNamingConvention>'), [ISupportNameResolution](ISupportNameResolution.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution'), [IApplicationBindingArtifactLookup](IApplicationBindingArtifactLookup.md 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingArtifactLookup'), [ISupportEnvironmentOverride](ISupportEnvironmentOverride.md 'Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation'), [Be.Stateless.BizTalk.Dsl.IVisitable&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.IVisitable-1 'Be.Stateless.BizTalk.Dsl.IVisitable`1')[IApplicationBindingVisitor](IApplicationBindingVisitor.md 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.IVisitable-1 'Be.Stateless.BizTalk.Dsl.IVisitable`1')

| Constructors | |
| :--- | :--- |
| [ApplicationBindingBase()](ApplicationBindingBase_TNamingConvention_.ApplicationBindingBase().md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.ApplicationBindingBase()') | |
| [ApplicationBindingBase(Action&lt;IApplicationBinding&lt;TNamingConvention&gt;&gt;)](ApplicationBindingBase_TNamingConvention_.ApplicationBindingBase(Action_IApplicationBinding_TNamingConvention__).md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.ApplicationBindingBase(System.Action<Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding<TNamingConvention>>)') | |

| Properties | |
| :--- | :--- |
| [Description](ApplicationBindingBase_TNamingConvention_.Description.md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.Description') | |
| [Name](ApplicationBindingBase_TNamingConvention_.Name.md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.Name') | |
| [Orchestrations](ApplicationBindingBase_TNamingConvention_.Orchestrations.md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.Orchestrations') | |
| [ReceivePorts](ApplicationBindingBase_TNamingConvention_.ReceivePorts.md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.ReceivePorts') | |
| [ReferencedApplications](ApplicationBindingBase_TNamingConvention_.ReferencedApplications.md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.ReferencedApplications') | |
| [SendPorts](ApplicationBindingBase_TNamingConvention_.SendPorts.md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.SendPorts') | |
| [Timestamp](ApplicationBindingBase_TNamingConvention_.Timestamp.md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.Timestamp') | |

| Methods | |
| :--- | :--- |
| [ApplyEnvironmentOverrides(string)](ApplicationBindingBase_TNamingConvention_.ApplyEnvironmentOverrides(string).md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.ApplyEnvironmentOverrides(string)') | |
| [ResolveName()](ApplicationBindingBase_TNamingConvention_.ResolveName().md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.ResolveName()') | |

| Explicit Interface Implementations | |
| :--- | :--- |
| [Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingArtifactLookup.ReceiveLocation&lt;T&gt;()](ApplicationBindingBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingArtifactLookup.ReceiveLocation_T_().md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingArtifactLookup.ReceiveLocation<T>()') | |
| [Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingArtifactLookup.ReceivePort&lt;T&gt;()](ApplicationBindingBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingArtifactLookup.ReceivePort_T_().md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingArtifactLookup.ReceivePort<T>()') | |
| [Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingArtifactLookup.ReferencedApplication&lt;T&gt;()](ApplicationBindingBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingArtifactLookup.ReferencedApplication_T_().md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingArtifactLookup.ReferencedApplication<T>()') | |
| [Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingArtifactLookup.SendPort&lt;T&gt;()](ApplicationBindingBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingArtifactLookup.SendPort_T_().md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingArtifactLookup.SendPort<T>()') | |
| [Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string)](ApplicationBindingBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string).md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string)') | |
| [Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate()](ApplicationBindingBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate()') | |
| [Be.Stateless.BizTalk.Dsl.IVisitable&lt;Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor&gt;.Accept&lt;TVisitor&gt;(TVisitor)](ApplicationBindingBase_TNamingConvention_.Be.Stateless.BizTalk.Dsl.IVisitable_Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor_.Accept_TVisitor_(TVisitor).md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.Be.Stateless.BizTalk.Dsl.IVisitable<Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor>.Accept<TVisitor>(TVisitor)') | |
| [Be.Stateless.BizTalk.IFluentInterface.GetType()](ApplicationBindingBase_TNamingConvention_.Be.Stateless.BizTalk.IFluentInterface.GetType().md 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBindingBase<TNamingConvention>.Be.Stateless.BizTalk.IFluentInterface.GetType()') | |
