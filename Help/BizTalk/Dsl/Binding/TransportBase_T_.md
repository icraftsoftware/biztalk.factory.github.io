#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding')

## TransportBase<T> Class

```csharp
public abstract class TransportBase<T> :
Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride,
Be.Stateless.BizTalk.IFluentInterface,
Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportHostResolution,
Be.Stateless.BizTalk.Dsl.ISupportValidation
    where T : class, Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter, Be.Stateless.BizTalk.Dsl.ISupportValidation
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.TransportBase_T_.T'></a>

`T`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; TransportBase<T>

Derived  
&#8627; [ReceiveLocationTransport&lt;TNamingConvention&gt;](ReceiveLocationTransport_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationTransport<TNamingConvention>')  
&#8627; [SendPortTransport&lt;TNamingConvention&gt;](SendPortTransport_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.SendPortTransport<TNamingConvention>')

Implements [ISupportEnvironmentOverride](ISupportEnvironmentOverride.md 'Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride'), [Be.Stateless.BizTalk.IFluentInterface](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.IFluentInterface 'Be.Stateless.BizTalk.IFluentInterface'), [ISupportHostResolution](ISupportHostResolution.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportHostResolution'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation')

| Properties | |
| :--- | :--- |
| [Adapter](TransportBase_T_.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.TransportBase<T>.Adapter') | |
| [Host](TransportBase_T_.Host.md 'Be.Stateless.BizTalk.Dsl.Binding.TransportBase<T>.Host') | The BizTalk Server Host Name that will host this transport's [Adapter](TransportBase_T_.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.TransportBase<T>.Adapter') at runtime. |

| Methods | |
| :--- | :--- |
| [ApplyEnvironmentOverrides(string)](TransportBase_T_.ApplyEnvironmentOverrides(string).md 'Be.Stateless.BizTalk.Dsl.Binding.TransportBase<T>.ApplyEnvironmentOverrides(string)') | |
| [ResolveHost()](TransportBase_T_.ResolveHost().md 'Be.Stateless.BizTalk.Dsl.Binding.TransportBase<T>.ResolveHost()') | Resolve host name that is to be bound to this transport's adapter. |

| Explicit Interface Implementations | |
| :--- | :--- |
| [Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string)](TransportBase_T_.Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string).md 'Be.Stateless.BizTalk.Dsl.Binding.TransportBase<T>.Be.Stateless.BizTalk.Dsl.Binding.ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string)') | |
| [Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate()](TransportBase_T_.Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.TransportBase<T>.Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate()') | |
| [Be.Stateless.BizTalk.IFluentInterface.GetType()](TransportBase_T_.Be.Stateless.BizTalk.IFluentInterface.GetType().md 'Be.Stateless.BizTalk.Dsl.Binding.TransportBase<T>.Be.Stateless.BizTalk.IFluentInterface.GetType()') | |
