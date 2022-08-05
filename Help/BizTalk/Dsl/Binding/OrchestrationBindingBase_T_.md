#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding')

## OrchestrationBindingBase<T> Class

```csharp
public abstract class OrchestrationBindingBase<T> :
Be.Stateless.BizTalk.Dsl.Binding.IOrchestrationBinding,
Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportHostResolution,
Be.Stateless.BizTalk.IFluentInterface,
Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution,
Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride,
Be.Stateless.BizTalk.Dsl.ISupportValidation,
Be.Stateless.BizTalk.Dsl.IVisitable<Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor>
    where T : Microsoft.BizTalk.XLANGs.BTXEngine.BTXService
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.OrchestrationBindingBase_T_.T'></a>

`T`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; OrchestrationBindingBase<T>

Implements [IOrchestrationBinding](IOrchestrationBinding.md 'Be.Stateless.BizTalk.Dsl.Binding.IOrchestrationBinding'), [ISupportHostResolution](ISupportHostResolution.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportHostResolution'), [Be.Stateless.BizTalk.IFluentInterface](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.IFluentInterface 'Be.Stateless.BizTalk.IFluentInterface'), [ISupportNameResolution](ISupportNameResolution.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportNameResolution'), [ISupportEnvironmentOverride](ISupportEnvironmentOverride.md 'Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation'), [Be.Stateless.BizTalk.Dsl.IVisitable&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.IVisitable-1 'Be.Stateless.BizTalk.Dsl.IVisitable`1')[IApplicationBindingVisitor](IApplicationBindingVisitor.md 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.IVisitable-1 'Be.Stateless.BizTalk.Dsl.IVisitable`1')

| Properties | |
| :--- | :--- |
| [ApplicationBinding](OrchestrationBindingBase_T_.ApplicationBinding.md 'Be.Stateless.BizTalk.Dsl.Binding.OrchestrationBindingBase<T>.ApplicationBinding') | |
| [Description](OrchestrationBindingBase_T_.Description.md 'Be.Stateless.BizTalk.Dsl.Binding.OrchestrationBindingBase<T>.Description') | |
| [Host](OrchestrationBindingBase_T_.Host.md 'Be.Stateless.BizTalk.Dsl.Binding.OrchestrationBindingBase<T>.Host') | |
| [PortBindings](OrchestrationBindingBase_T_.PortBindings.md 'Be.Stateless.BizTalk.Dsl.Binding.OrchestrationBindingBase<T>.PortBindings') | |
| [State](OrchestrationBindingBase_T_.State.md 'Be.Stateless.BizTalk.Dsl.Binding.OrchestrationBindingBase<T>.State') | |
| [Type](OrchestrationBindingBase_T_.Type.md 'Be.Stateless.BizTalk.Dsl.Binding.OrchestrationBindingBase<T>.Type') | |

| Methods | |
| :--- | :--- |
| [ApplyEnvironmentOverrides(string)](OrchestrationBindingBase_T_.ApplyEnvironmentOverrides(string).md 'Be.Stateless.BizTalk.Dsl.Binding.OrchestrationBindingBase<T>.ApplyEnvironmentOverrides(string)') | |
| [ResolveHost()](OrchestrationBindingBase_T_.ResolveHost().md 'Be.Stateless.BizTalk.Dsl.Binding.OrchestrationBindingBase<T>.ResolveHost()') | |
| [ResolveName()](OrchestrationBindingBase_T_.ResolveName().md 'Be.Stateless.BizTalk.Dsl.Binding.OrchestrationBindingBase<T>.ResolveName()') | |

| Explicit Interface Implementations | |
| :--- | :--- |
| [Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string)](OrchestrationBindingBase_T_.Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string).md 'Be.Stateless.BizTalk.Dsl.Binding.OrchestrationBindingBase<T>.Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string)') | |
| [Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate()](OrchestrationBindingBase_T_.Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.OrchestrationBindingBase<T>.Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate()') | |
| [Be.Stateless.BizTalk.Dsl.IVisitable&lt;Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor&gt;.Accept&lt;TVisitor&gt;(TVisitor)](OrchestrationBindingBase_T_.Be.Stateless.BizTalk.Dsl.IVisitable_Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor_.Accept_TVisitor_(TVisitor).md 'Be.Stateless.BizTalk.Dsl.Binding.OrchestrationBindingBase<T>.Be.Stateless.BizTalk.Dsl.IVisitable<Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor>.Accept<TVisitor>(TVisitor)') | |
| [Be.Stateless.BizTalk.IFluentInterface.GetType()](OrchestrationBindingBase_T_.Be.Stateless.BizTalk.IFluentInterface.GetType().md 'Be.Stateless.BizTalk.Dsl.Binding.OrchestrationBindingBase<T>.Be.Stateless.BizTalk.IFluentInterface.GetType()') | |
