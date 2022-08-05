#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Processing](Be.Stateless.BizTalk.Activity.Tracking.Processing.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing').[ProcessingStep](ProcessingStep.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep')

## ProcessingStep.Fail(TrackingContext, Exception) Method

Method to be called at the end of a failed orchestration processing step.

```csharp
public static void Fail(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext trackingContext, System.Exception exception);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep.Fail(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,System.Exception).trackingContext'></a>

`trackingContext` [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')

[TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')
            Structure containing the appropriate activity identifiers.

<a name='Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep.Fail(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,System.Exception).exception'></a>

`exception` [System.Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Exception 'System.Exception')

The exception that causes the processing step to fail.

### Remarks
It will end the processing step activity, setting its [Status](ProcessingStep.Status.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep.Status') to [Failed](TrackingStatus.Failed.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingStatus.Failed').