#### [Be.Stateless.BizTalk.Pipeline.Components.NUnit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Component](Be.Stateless.BizTalk.Unit.Component.md 'Be.Stateless.BizTalk.Unit.Component')

## PipelineComponentFixture<T> Class

Base class that all [Be.Stateless.BizTalk.Component.PipelineComponent](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Component.PipelineComponent 'Be.Stateless.BizTalk.Component.PipelineComponent') fixtures written against `NUnit` should inherit from.

```csharp
public abstract class PipelineComponentFixture<T> : Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase<T>
    where T : Be.Stateless.BizTalk.Component.PipelineComponent, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixture_T_.T'></a>

`T`

The [Be.Stateless.BizTalk.Component.PipelineComponent](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Component.PipelineComponent 'Be.Stateless.BizTalk.Component.PipelineComponent') derived class to test.

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase-1 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase`1')[T](PipelineComponentFixture_T_.md#Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixture_T_.T 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixture<T>.T')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase-1 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase`1') &#129106; PipelineComponentFixture<T>

### Remarks
This is essentially a `NUnit` tailored version of the [Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase-1 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase`1') base class.

### See Also
- [Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase-1 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase`1')

| Methods | |
| :--- | :--- |
| [AllPropertiesAreLoadedFromPropertyBag()](PipelineComponentFixture_T_.AllPropertiesAreLoadedFromPropertyBag().md 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixture<T>.AllPropertiesAreLoadedFromPropertyBag()') | |
| [AllPropertiesAreSavedToPropertyBag()](PipelineComponentFixture_T_.AllPropertiesAreSavedToPropertyBag().md 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixture<T>.AllPropertiesAreSavedToPropertyBag()') | |
| [AllPropertiesSupportRoundTripStringConversion()](PipelineComponentFixture_T_.AllPropertiesSupportRoundTripStringConversion().md 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixture<T>.AllPropertiesSupportRoundTripStringConversion()') | |
| [ExecuteCoreIsSkippedWhenPipelineComponentIsNotEnabled()](PipelineComponentFixture_T_.ExecuteCoreIsSkippedWhenPipelineComponentIsNotEnabled().md 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixture<T>.ExecuteCoreIsSkippedWhenPipelineComponentIsNotEnabled()') | |
| [ExecuteReturnsImmediatelyWhenMessageIsNull()](PipelineComponentFixture_T_.ExecuteReturnsImmediatelyWhenMessageIsNull().md 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixture<T>.ExecuteReturnsImmediatelyWhenMessageIsNull()') | |
| [ExecuteThrowsWhenPipelineContextIsNull()](PipelineComponentFixture_T_.ExecuteThrowsWhenPipelineContextIsNull().md 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixture<T>.ExecuteThrowsWhenPipelineContextIsNull()') | |
| [PipelineComponentFixtureOfTSetUp()](PipelineComponentFixture_T_.PipelineComponentFixtureOfTSetUp().md 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixture<T>.PipelineComponentFixtureOfTSetUp()') | |
