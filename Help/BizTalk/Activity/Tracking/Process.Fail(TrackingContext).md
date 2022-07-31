#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Processing](Be.Stateless.BizTalk.Activity.Tracking.Processing.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing').[Process](Process.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process')

## Process.Fail(TrackingContext) Method

Method intended to be called at the end of a failed orchestration to end its corresponding BAM process tracking
activity.

```csharp
public static void Fail(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext trackingContext);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.Fail(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext).trackingContext'></a>

`trackingContext` [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')

[TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')
            Structure containing the appropriate activity identifiers.

### Remarks
Method to be called at the end of a process, it will end the process activity and set its [Status](Process.Status.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.Status') to [Failed](TrackingStatus.Failed.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingStatus.Failed').