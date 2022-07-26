#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent')

## ContextBuilder Class

Delegates building of message context to a [IContextBuilder](IContextBuilder.md 'Be.Stateless.BizTalk.MicroComponent.IContextBuilder') component plugin.

```csharp
public class ContextBuilder :
Be.Stateless.BizTalk.MicroComponent.IMicroComponent
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ContextBuilder

Implements [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')

| Properties | |
| :--- | :--- |
| [BuilderType](ContextBuilder.BuilderType.md 'Be.Stateless.BizTalk.MicroComponent.ContextBuilder.BuilderType') | The type name of the context builder plugin that will be called upon. |
| [ExecutionTime](ContextBuilder.ExecutionTime.md 'Be.Stateless.BizTalk.MicroComponent.ContextBuilder.ExecutionTime') | The plugin execution mode, either [Immediate](PluginExecutionTime.md#Be.Stateless.BizTalk.PluginExecutionTime.Immediate 'Be.Stateless.BizTalk.PluginExecutionTime.Immediate') or [Deferred](PluginExecutionTime.md#Be.Stateless.BizTalk.PluginExecutionTime.Deferred 'Be.Stateless.BizTalk.PluginExecutionTime.Deferred'). |

| Methods | |
| :--- | :--- |
| [Execute(IPipelineContext, IBaseMessage)](ContextBuilder.Execute(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.MicroComponent.ContextBuilder.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
