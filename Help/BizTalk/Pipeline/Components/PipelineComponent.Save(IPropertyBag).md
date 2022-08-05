#### [Be.Stateless.BizTalk.Pipeline.Components](README.md 'README')
### [Be.Stateless.BizTalk.Component](Be.Stateless.BizTalk.Component.md 'Be.Stateless.BizTalk.Component').[PipelineComponent](PipelineComponent.md 'Be.Stateless.BizTalk.Component.PipelineComponent')

## PipelineComponent.Save(IPropertyBag) Method

Saves the pipeline component configuration. This base class implementation must be called by derived classes if they
override it.

```csharp
protected abstract void Save(Microsoft.BizTalk.Component.Interop.IPropertyBag propertyBag);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Component.PipelineComponent.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag).propertyBag'></a>

`propertyBag` [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag')