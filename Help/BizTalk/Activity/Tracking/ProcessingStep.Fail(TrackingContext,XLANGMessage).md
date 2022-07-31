#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Processing](Be.Stateless.BizTalk.Activity.Tracking.Processing.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing').[ProcessingStep](ProcessingStep.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep')

## ProcessingStep.Fail(TrackingContext, XLANGMessage) Method

Method to be called at the end of a failed orchestration processing step.

```csharp
public static void Fail(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext trackingContext, Microsoft.XLANGs.BaseTypes.XLANGMessage faultMessage);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep.Fail(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,Microsoft.XLANGs.BaseTypes.XLANGMessage).trackingContext'></a>

`trackingContext` [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')

[TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')
            Structure containing the appropriate activity identifiers.

<a name='Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep.Fail(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,Microsoft.XLANGs.BaseTypes.XLANGMessage).faultMessage'></a>

`faultMessage` [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')

The fault message that causes the processing step to fail.

### Remarks
It will end the processing step activity, setting its [Status](ProcessingStep.Status.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep.Status') to [Failed](TrackingStatus.Failed.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingStatus.Failed').