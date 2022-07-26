#### [Be.Stateless.BizTalk.Pipeline.MicroComponents.NUnit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.MicroComponent](Be.Stateless.BizTalk.Unit.MicroComponent.md 'Be.Stateless.BizTalk.Unit.MicroComponent')

## MicroComponentFixture<T> Class

Base class that all fixtures written against `NUnit` should inherit when testing [Be.Stateless.BizTalk.MicroComponent.IMicroComponent](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.MicroComponent.IMicroComponent 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')-derived classes.

```csharp
public abstract class MicroComponentFixture<T> : Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase<T>
    where T : Be.Stateless.BizTalk.MicroComponent.IMicroComponent
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixture_T_.T'></a>

`T`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase-1 'Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase`1')[T](MicroComponentFixture_T_.md#Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixture_T_.T 'Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixture<T>.T')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase-1 'Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase`1') &#129106; MicroComponentFixture<T>

### Remarks
This is essentially a `NUnit` tailored version of the [Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase-1 'Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase`1') base class.

### See Also
- [Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase-1 'Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixtureBase`1')

| Methods | |
| :--- | :--- |
| [MicroComponentFixtureSetUp()](MicroComponentFixture_T_.MicroComponentFixtureSetUp().md 'Be.Stateless.BizTalk.Unit.MicroComponent.MicroComponentFixture<T>.MicroComponentFixtureSetUp()') | |
