#### [Be.Stateless.BizTalk.Pipeline.Components](README.md 'README')
### [Be.Stateless.BizTalk.Component](Be.Stateless.BizTalk.Component.md 'Be.Stateless.BizTalk.Component')

## PipelineComponent Class

Base class for BizTalk Server pipeline components.

```csharp
public abstract class PipelineComponent :
Microsoft.BizTalk.Component.Interop.IBaseComponent,
Microsoft.BizTalk.Component.Interop.IComponent,
Microsoft.BizTalk.Component.Interop.IComponentUI,
Microsoft.BizTalk.Component.Interop.IPersistPropertyBag
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; PipelineComponent

Derived  
&#8627; [FailedMessageRoutingEnablerComponent](FailedMessageRoutingEnablerComponent.md 'Be.Stateless.BizTalk.Component.FailedMessageRoutingEnablerComponent')  
&#8627; [MicroPipelineComponent](MicroPipelineComponent.md 'Be.Stateless.BizTalk.Component.MicroPipelineComponent')

Implements [Microsoft.BizTalk.Component.Interop.IBaseComponent](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IBaseComponent 'Microsoft.BizTalk.Component.Interop.IBaseComponent'), [Microsoft.BizTalk.Component.Interop.IComponent](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IComponent 'Microsoft.BizTalk.Component.Interop.IComponent'), [Microsoft.BizTalk.Component.Interop.IComponentUI](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IComponentUI 'Microsoft.BizTalk.Component.Interop.IComponentUI'), [Microsoft.BizTalk.Component.Interop.IPersistPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPersistPropertyBag 'Microsoft.BizTalk.Component.Interop.IPersistPropertyBag')

| Properties | |
| :--- | :--- |
| [Description](PipelineComponent.Description.md 'Be.Stateless.BizTalk.Component.PipelineComponent.Description') | Description of the pipeline component. |
| [Enabled](PipelineComponent.Enabled.md 'Be.Stateless.BizTalk.Component.PipelineComponent.Enabled') | Enables or disables the pipeline component. |
| [Icon](PipelineComponent.Icon.md 'Be.Stateless.BizTalk.Component.PipelineComponent.Icon') | Component icon to use in BizTalk Editor. |
| [Name](PipelineComponent.Name.md 'Be.Stateless.BizTalk.Component.PipelineComponent.Name') | Name of the pipeline component. |
| [Version](PipelineComponent.Version.md 'Be.Stateless.BizTalk.Component.PipelineComponent.Version') | Version of the pipeline component. |

| Methods | |
| :--- | :--- |
| [Execute(IPipelineContext, IBaseMessage)](PipelineComponent.Execute(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.Component.PipelineComponent.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | Executes a pipeline component to process the input message and get the resulting message. |
| [ExecuteCore(IPipelineContext, IBaseMessage)](PipelineComponent.ExecuteCore(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.Component.PipelineComponent.ExecuteCore(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | Executes a pipeline component to process the input message and get the resulting message. |
| [GetClassID(Guid)](PipelineComponent.GetClassID(Guid).md 'Be.Stateless.BizTalk.Component.PipelineComponent.GetClassID(System.Guid)') | |
| [Load(IPropertyBag, int)](PipelineComponent.Load(IPropertyBag,int).md 'Be.Stateless.BizTalk.Component.PipelineComponent.Load(Microsoft.BizTalk.Component.Interop.IPropertyBag, int)') | Loads the pipeline component configuration. This base class implementation must be called by derived classes if they override it. |
| [Load(IPropertyBag)](PipelineComponent.Load(IPropertyBag).md 'Be.Stateless.BizTalk.Component.PipelineComponent.Load(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | Loads configuration properties for the component |
| [Save(IPropertyBag, bool, bool)](PipelineComponent.Save(IPropertyBag,bool,bool).md 'Be.Stateless.BizTalk.Component.PipelineComponent.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag, bool, bool)') | Saves the pipeline component configuration. This base class implementation must be called by derived classes if they override it. |
| [Save(IPropertyBag)](PipelineComponent.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Component.PipelineComponent.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | Saves the pipeline component configuration. This base class implementation must be called by derived classes if they override it. |
| [Validate(object)](PipelineComponent.Validate(object).md 'Be.Stateless.BizTalk.Component.PipelineComponent.Validate(object)') | The Validate method is called by the BizTalk Editor during the build of a BizTalk project. |

| Explicit Interface Implementations | |
| :--- | :--- |
| [Microsoft.BizTalk.Component.Interop.IPersistPropertyBag.InitNew()](PipelineComponent.Microsoft.BizTalk.Component.Interop.IPersistPropertyBag.InitNew().md 'Be.Stateless.BizTalk.Component.PipelineComponent.Microsoft.BizTalk.Component.Interop.IPersistPropertyBag.InitNew()') | Not implemented |
