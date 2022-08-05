#### [Be.Stateless.BizTalk.Pipeline.Components.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Component](Be.Stateless.BizTalk.Unit.Component.md 'Be.Stateless.BizTalk.Unit.Component').[PipelineComponentFixtureBase&lt;T&gt;](PipelineComponentFixtureBase_T_.md 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase<T>')

## PipelineComponentFixtureBase<T>.VerifyAllPropertiesSupportRoundTripStringConversion() Method

Ensure all	[ConfigurableProperties](PipelineComponentFixtureBase_T_.ConfigurableProperties.md 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase<T>.ConfigurableProperties') can be converted back and forth to a string in order to be both
readable from and writable to an [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag').

```csharp
protected void VerifyAllPropertiesSupportRoundTripStringConversion();
```