#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent')

## FailedMessageRoutingEnabler Class

Enables routing of failed messages and prevents routing failure reports from being generated.

```csharp
public class FailedMessageRoutingEnabler :
Be.Stateless.BizTalk.MicroComponent.IMicroComponent
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; FailedMessageRoutingEnabler

Implements [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')

| Properties | |
| :--- | :--- |
| [EnableFailedMessageRouting](FailedMessageRoutingEnabler.EnableFailedMessageRouting.md 'Be.Stateless.BizTalk.MicroComponent.FailedMessageRoutingEnabler.EnableFailedMessageRouting') | Enables or disables routing of failed messages and whether to avoid suspended message instances. |
| [SuppressRoutingFailureReport](FailedMessageRoutingEnabler.SuppressRoutingFailureReport.md 'Be.Stateless.BizTalk.MicroComponent.FailedMessageRoutingEnabler.SuppressRoutingFailureReport') | Whether to prevent the generation of a routing failure report upon message routing failure. |

| Methods | |
| :--- | :--- |
| [Execute(IPipelineContext, IBaseMessage)](FailedMessageRoutingEnabler.Execute(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.MicroComponent.FailedMessageRoutingEnabler.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
