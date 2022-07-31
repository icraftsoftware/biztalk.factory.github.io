#### [Be.Stateless.BizTalk.Pipeline.Components](README.md 'README')
### [Be.Stateless.BizTalk.Component](Be.Stateless.BizTalk.Component.md 'Be.Stateless.BizTalk.Component')

## FailedMessageRoutingEnablerComponent Class

Enables routing of failed messages and prevents routing failure reports from being generated.

```csharp
public class FailedMessageRoutingEnablerComponent : Be.Stateless.BizTalk.Component.PipelineComponent
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [PipelineComponent](PipelineComponent.md 'Be.Stateless.BizTalk.Component.PipelineComponent') &#129106; FailedMessageRoutingEnablerComponent

| Properties | |
| :--- | :--- |
| [Description](FailedMessageRoutingEnablerComponent.Description.md 'Be.Stateless.BizTalk.Component.FailedMessageRoutingEnablerComponent.Description') | Description of the pipeline component. |
| [EnableFailedMessageRouting](FailedMessageRoutingEnablerComponent.EnableFailedMessageRouting.md 'Be.Stateless.BizTalk.Component.FailedMessageRoutingEnablerComponent.EnableFailedMessageRouting') | Enables or disables routing of failed messages and whether to avoid suspended message instances. |
| [SuppressRoutingFailureReport](FailedMessageRoutingEnablerComponent.SuppressRoutingFailureReport.md 'Be.Stateless.BizTalk.Component.FailedMessageRoutingEnablerComponent.SuppressRoutingFailureReport') | Whether to prevent the generation of a routing failure report upon message routing failure. |

| Methods | |
| :--- | :--- |
| [ExecuteCore(IPipelineContext, IBaseMessage)](FailedMessageRoutingEnablerComponent.ExecuteCore(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.Component.FailedMessageRoutingEnablerComponent.ExecuteCore(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
| [GetClassID(Guid)](FailedMessageRoutingEnablerComponent.GetClassID(Guid).md 'Be.Stateless.BizTalk.Component.FailedMessageRoutingEnablerComponent.GetClassID(System.Guid)') | Gets class ID of component for usage from unmanaged code. |
| [Load(IPropertyBag)](FailedMessageRoutingEnablerComponent.Load(IPropertyBag).md 'Be.Stateless.BizTalk.Component.FailedMessageRoutingEnablerComponent.Load(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | Loads configuration properties for the component |
| [Save(IPropertyBag)](FailedMessageRoutingEnablerComponent.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Component.FailedMessageRoutingEnablerComponent.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | Saves the current component configuration into the property bag |
