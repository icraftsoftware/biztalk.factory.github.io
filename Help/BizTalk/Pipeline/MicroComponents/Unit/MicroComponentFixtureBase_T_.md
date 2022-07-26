#### [Be.Stateless.BizTalk.Pipeline.MicroComponents.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.MicroComponent](Be.Stateless.BizTalk.Unit.MicroComponent.md 'Be.Stateless.BizTalk.Unit.MicroComponent')

## MicroComponentFixtureBase<T> Class

This base class provides utility methods for [Be.Stateless.BizTalk.MicroComponent.IMicroComponent](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.MicroComponent.IMicroComponent 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')-derived classes.

```csharp
public abstract class MicroComponentFixtureBase<T>
    where T : Be.Stateless.BizTalk.MicroComponent.IMicroComponent
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase_T_.T'></a>

`T`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; MicroComponentFixtureBase<T>

| Properties | |
| :--- | :--- |
| [MessageMock](MicroComponentFixtureBase_T_.MessageMock.md 'Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase<T>.MessageMock') | |
| [PipelineContextMock](MicroComponentFixtureBase_T_.PipelineContextMock.md 'Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase<T>.PipelineContextMock') | |

| Methods | |
| :--- | :--- |
| [Initialize()](MicroComponentFixtureBase_T_.Initialize().md 'Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase<T>.Initialize()') | [MicroComponentFixtureBase&lt;T&gt;](MicroComponentFixtureBase_T_.md 'Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase<T>') initialization to be called either by an xUnit fixture's constructor or a             NUnit fixture's SetUp method. |
