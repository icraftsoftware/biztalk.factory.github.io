#### [Be.Stateless.BizTalk.Pipeline.Components.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Component](Be.Stateless.BizTalk.Unit.Component.md 'Be.Stateless.BizTalk.Unit.Component').[PipelineComponentFixtureBase&lt;T&gt;](PipelineComponentFixtureBase_T_.md 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase<T>')

## PipelineComponentFixtureBase<T>.VerifyAllPropertiesAreLoadedFromPropertyBag() Method

Ensure all [ConfigurableProperties](PipelineComponentFixtureBase_T_.ConfigurableProperties.md 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase<T>.ConfigurableProperties') are loaded from an [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag'), it mainly protects
pipeline component authors from stupid copy/paste mistakes in [Be.Stateless.BizTalk.Component.PipelineComponent](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Component.PipelineComponent 'Be.Stateless.BizTalk.Component.PipelineComponent')-derived classes.

```csharp
protected void VerifyAllPropertiesAreLoadedFromPropertyBag();
```