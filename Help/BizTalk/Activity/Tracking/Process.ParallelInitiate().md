#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Processing](Be.Stateless.BizTalk.Activity.Tracking.Processing.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing').[Process](Process.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process')

## Process.ParallelInitiate() Method

Method intended to be called near the start of an orchestration after all of its activating parallel receives ([ParallelPreInitiate(XLANGMessage)](Process.ParallelPreInitiate(XLANGMessage).md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.ParallelPreInitiate(Microsoft.XLANGs.BaseTypes.XLANGMessage)')) have completed, or failed, to create a BAM process tracking activity.

```csharp
public static Be.Stateless.BizTalk.Activity.Tracking.TrackingContext ParallelInitiate();
```

#### Returns
[TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')  
The [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') that contains the BAM tracking activities identifiers for the current process.
Notice that, contrary to [Initiate(XLANGMessage)](Process.Initiate(XLANGMessage).md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.Initiate(Microsoft.XLANGs.BaseTypes.XLANGMessage)'), [MessagingStepActivityId](TrackingContext.MessagingStepActivityId.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext.MessagingStepActivityId')
will not be filled.

### Remarks
The BAM process tracking activity, whose parallel activating messages have already all been received ([ParallelPreInitiate(XLANGMessage)](Process.ParallelPreInitiate(XLANGMessage).md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.ParallelPreInitiate(Microsoft.XLANGs.BaseTypes.XLANGMessage)')), will be created thereby providing the missing half of the process-to-activating
messages associations. The name used for the process instance is the containing namespace of the calling
orchestration.