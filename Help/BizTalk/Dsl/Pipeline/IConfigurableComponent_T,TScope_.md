#### [Be.Stateless.BizTalk.Dsl.Pipeline](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Pipeline](Be.Stateless.BizTalk.Dsl.Pipeline.md 'Be.Stateless.BizTalk.Dsl.Pipeline')

## IConfigurableComponent<T,TScope> Interface

```csharp
public interface IConfigurableComponent<out T,out TScope> :
Be.Stateless.BizTalk.IFluentInterface
    where T : Microsoft.BizTalk.Component.Interop.IBaseComponent, Microsoft.BizTalk.Component.Interop.IPersistPropertyBag
    where TScope : Be.Stateless.BizTalk.IFluentInterface
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Pipeline.IConfigurableComponent_T,TScope_.T'></a>

`T`

<a name='Be.Stateless.BizTalk.Dsl.Pipeline.IConfigurableComponent_T,TScope_.TScope'></a>

`TScope`

Implements [Be.Stateless.BizTalk.IFluentInterface](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.IFluentInterface 'Be.Stateless.BizTalk.IFluentInterface')

| Methods | |
| :--- | :--- |
| [Configure(Action&lt;T&gt;)](IConfigurableComponent_T,TScope_.Configure(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.IConfigurableComponent<T,TScope>.Configure(System.Action<T>)') | |
