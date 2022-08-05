#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking](Be.Stateless.BizTalk.Activity.Tracking.md 'Be.Stateless.BizTalk.Activity.Tracking')

## TrackingContext Struct

Simple structure that holds the BAM activity identifiers of the activities used for tracking at the process, processing
step, and messaging step levels.

```csharp
public struct TrackingContext
```

| Properties | |
| :--- | :--- |
| [MessagingStepActivityId](TrackingContext.MessagingStepActivityId.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext.MessagingStepActivityId') | The identifier of the BAM messaging step activity. |
| [ProcessActivityId](TrackingContext.ProcessActivityId.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext.ProcessActivityId') | The identifier of the BAM process activity. |
| [ProcessingStepActivityId](TrackingContext.ProcessingStepActivityId.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext.ProcessingStepActivityId') | The identifier of the BAM processing step activity. |

| Methods | |
| :--- | :--- |
| [Apply(XLANGMessage)](TrackingContext.Apply(XLANGMessage).md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext.Apply(Microsoft.XLANGs.BaseTypes.XLANGMessage)') | Applies this [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') instance to the [targetMessage](TrackingContext.Apply(XLANGMessage).md#Be.Stateless.BizTalk.Activity.Tracking.TrackingContext.Apply(Microsoft.XLANGs.BaseTypes.XLANGMessage).targetMessage 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext.Apply(Microsoft.XLANGs.BaseTypes.XLANGMessage).targetMessage'). |
| [HasProcessAffiliation()](TrackingContext.HasProcessAffiliation().md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext.HasProcessAffiliation()') | Whether the current [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') is already affiliated to a process or not. |
| [IsEmpty()](TrackingContext.IsEmpty().md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext.IsEmpty()') | Whether none of the discrete activity Ids of the [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') are set or not. |
