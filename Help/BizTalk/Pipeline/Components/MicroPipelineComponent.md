#### [Be.Stateless.BizTalk.Pipeline.Components](README.md 'README')
### [Be.Stateless.BizTalk.Component](Be.Stateless.BizTalk.Component.md 'Be.Stateless.BizTalk.Component')

## MicroPipelineComponent Class

Runs a sequence of micro components, i.e. components implementing [Be.Stateless.BizTalk.MicroComponent.IMicroComponent](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.MicroComponent.IMicroComponent 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent'), similarly to what a
regular Microsoft BizTalk Server pipeline would do if the micro components were regular pipeline components.

```csharp
public class MicroPipelineComponent : Be.Stateless.BizTalk.Component.PipelineComponent
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [PipelineComponent](PipelineComponent.md 'Be.Stateless.BizTalk.Component.PipelineComponent') &#129106; MicroPipelineComponent

| Properties | |
| :--- | :--- |
| [Components](MicroPipelineComponent.Components.md 'Be.Stateless.BizTalk.Component.MicroPipelineComponent.Components') | List of micro components that will be run in sequence by the micro pipeline. |
| [Description](MicroPipelineComponent.Description.md 'Be.Stateless.BizTalk.Component.MicroPipelineComponent.Description') | Description of the pipeline component. |

| Methods | |
| :--- | :--- |
| [ExecuteCore(IPipelineContext, IBaseMessage)](MicroPipelineComponent.ExecuteCore(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.Component.MicroPipelineComponent.ExecuteCore(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
| [GetClassID(Guid)](MicroPipelineComponent.GetClassID(Guid).md 'Be.Stateless.BizTalk.Component.MicroPipelineComponent.GetClassID(System.Guid)') | Gets class ID of component for usage from unmanaged code. |
| [Load(IPropertyBag)](MicroPipelineComponent.Load(IPropertyBag).md 'Be.Stateless.BizTalk.Component.MicroPipelineComponent.Load(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | Loads configuration properties for the component from the [propertyBag](MicroPipelineComponent.Load(IPropertyBag).md#Be.Stateless.BizTalk.Component.MicroPipelineComponent.Load(Microsoft.BizTalk.Component.Interop.IPropertyBag).propertyBag 'Be.Stateless.BizTalk.Component.MicroPipelineComponent.Load(Microsoft.BizTalk.Component.Interop.IPropertyBag).propertyBag'). |
| [Save(IPropertyBag)](MicroPipelineComponent.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Component.MicroPipelineComponent.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | Saves the current component configuration to the [propertyBag](MicroPipelineComponent.Save(IPropertyBag).md#Be.Stateless.BizTalk.Component.MicroPipelineComponent.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag).propertyBag 'Be.Stateless.BizTalk.Component.MicroPipelineComponent.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag).propertyBag'). |
