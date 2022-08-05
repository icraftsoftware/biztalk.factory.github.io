#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Processing](Be.Stateless.BizTalk.Activity.Tracking.Processing.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing').[ProcessingStep](ProcessingStep.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep')

## ProcessingStep.Complete(TrackingContext) Method

Method to be called at the end of a successful orchestration processing step.

```csharp
public static void Complete(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext trackingContext);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep.Complete(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext).trackingContext'></a>

`trackingContext` [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')

[TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')
            Structure containing the appropriate activity identifiers.

### Remarks
It will end the processing step activity, setting its [Status](ProcessingStep.Status.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep.Status') to [Completed](TrackingStatus.Completed.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingStatus.Completed'),
but will not end the process activity.