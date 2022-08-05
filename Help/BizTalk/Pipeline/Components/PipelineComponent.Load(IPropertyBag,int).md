#### [Be.Stateless.BizTalk.Pipeline.Components](README.md 'README')
### [Be.Stateless.BizTalk.Component](Be.Stateless.BizTalk.Component.md 'Be.Stateless.BizTalk.Component').[PipelineComponent](PipelineComponent.md 'Be.Stateless.BizTalk.Component.PipelineComponent')

## PipelineComponent.Load(IPropertyBag, int) Method

Loads the pipeline component configuration. This base class implementation must be called by derived classes if they
override it.

```csharp
public void Load(Microsoft.BizTalk.Component.Interop.IPropertyBag propertyBag, int errorLog);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Component.PipelineComponent.Load(Microsoft.BizTalk.Component.Interop.IPropertyBag,int).propertyBag'></a>

`propertyBag` [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag')

<a name='Be.Stateless.BizTalk.Component.PipelineComponent.Load(Microsoft.BizTalk.Component.Interop.IPropertyBag,int).errorLog'></a>

`errorLog` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

Implements [Load(IPropertyBag, int)](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPersistPropertyBag.Load#Microsoft_BizTalk_Component_Interop_IPersistPropertyBag_Load_Microsoft_BizTalk_Component_Interop_IPropertyBag,System_Int32_ 'Microsoft.BizTalk.Component.Interop.IPersistPropertyBag.Load(Microsoft.BizTalk.Component.Interop.IPropertyBag,System.Int32)')