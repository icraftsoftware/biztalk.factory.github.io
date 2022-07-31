#### [Be.Stateless.BizTalk.Pipeline.Components](README.md 'README')
### [Be.Stateless.BizTalk.Component](Be.Stateless.BizTalk.Component.md 'Be.Stateless.BizTalk.Component').[PipelineComponent](PipelineComponent.md 'Be.Stateless.BizTalk.Component.PipelineComponent')

## PipelineComponent.Save(IPropertyBag, bool, bool) Method

Saves the pipeline component configuration. This base class implementation must be called by derived classes if they
override it.

```csharp
public void Save(Microsoft.BizTalk.Component.Interop.IPropertyBag propertyBag, bool clearDirty, bool saveAllProperties);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Component.PipelineComponent.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag,bool,bool).propertyBag'></a>

`propertyBag` [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag')

<a name='Be.Stateless.BizTalk.Component.PipelineComponent.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag,bool,bool).clearDirty'></a>

`clearDirty` [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

<a name='Be.Stateless.BizTalk.Component.PipelineComponent.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag,bool,bool).saveAllProperties'></a>

`saveAllProperties` [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

Implements [Save(IPropertyBag, bool, bool)](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPersistPropertyBag.Save#Microsoft_BizTalk_Component_Interop_IPersistPropertyBag_Save_Microsoft_BizTalk_Component_Interop_IPropertyBag,System_Boolean,System_Boolean_ 'Microsoft.BizTalk.Component.Interop.IPersistPropertyBag.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag,System.Boolean,System.Boolean)')