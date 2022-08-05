#### [Be.Stateless.BizTalk.Dsl.Pipeline](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Pipeline](Be.Stateless.BizTalk.Dsl.Pipeline.md 'Be.Stateless.BizTalk.Dsl.Pipeline').[IStage](IStage.md 'Be.Stateless.BizTalk.Dsl.Pipeline.IStage')

## IStage.AddComponent<T>(Action<T>) Method

```csharp
Be.Stateless.BizTalk.Dsl.Pipeline.IStage AddComponent<T>(System.Action<T> componentConfigurator)
    where T : Microsoft.BizTalk.Component.Interop.IBaseComponent, Microsoft.BizTalk.Component.Interop.IComponentUI, Microsoft.BizTalk.Component.Interop.IPersistPropertyBag, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Pipeline.IStage.AddComponent_T_(System.Action_T_).T'></a>

`T`
#### Parameters

<a name='Be.Stateless.BizTalk.Dsl.Pipeline.IStage.AddComponent_T_(System.Action_T_).componentConfigurator'></a>

`componentConfigurator` [System.Action&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')[T](IStage.AddComponent_T_(Action_T_).md#Be.Stateless.BizTalk.Dsl.Pipeline.IStage.AddComponent_T_(System.Action_T_).T 'Be.Stateless.BizTalk.Dsl.Pipeline.IStage.AddComponent<T>(System.Action<T>).T')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')

#### Returns
[IStage](IStage.md 'Be.Stateless.BizTalk.Dsl.Pipeline.IStage')