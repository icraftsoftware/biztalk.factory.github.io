#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent')

## ActivityTracker Class

Tracks process and messaging step activities altogether and feeds the BAM tracking activity model and ensures the
automatic propagation of the activity tracking context for solicit-response ports as well.

```csharp
public class ActivityTracker :
Be.Stateless.BizTalk.MicroComponent.IMicroComponent
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ActivityTracker

Implements [Be.Stateless.BizTalk.MicroComponent.IMicroComponent](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.MicroComponent.IMicroComponent 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')

| Properties | |
| :--- | :--- |
| [TrackingContextCacheDuration](ActivityTracker.TrackingContextCacheDuration.md 'Be.Stateless.BizTalk.MicroComponent.ActivityTracker.TrackingContextCacheDuration') | How long activity tracking contexts will be kept in cache when propagated through solicit-response ports. Any negative value disables caching. |
| [TrackingModes](ActivityTracker.TrackingModes.md 'Be.Stateless.BizTalk.MicroComponent.ActivityTracker.TrackingModes') | Level of tracking to use, or the extent of message data to capture. |

| Methods | |
| :--- | :--- |
| [Execute(IPipelineContext, IBaseMessage)](ActivityTracker.Execute(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.MicroComponent.ActivityTracker.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
