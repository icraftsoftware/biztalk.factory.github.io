#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Processing](Be.Stateless.BizTalk.Activity.Tracking.Processing.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing').[ProcessingStep](ProcessingStep.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep')

## ProcessingStep.Initiate(TrackingContext, string) Method

Method intended to be called when starting a processing step in the middle of an orchestration. It is expected that a
tracking context has been created previously, at the start of the orchestration by a call to [Initiate(XLANGMessage)](Process.Initiate(XLANGMessage).md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.Initiate(Microsoft.XLANGs.BaseTypes.XLANGMessage)') or by a call to this method. A new processing step tracking activity is
always started, and it is always linked to the process tracking activity identified in [trackingContext](ProcessingStep.Initiate(TrackingContext,string).md#Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep.Initiate(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,string).trackingContext 'Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep.Initiate(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext, string).trackingContext').

```csharp
public static Be.Stateless.BizTalk.Activity.Tracking.TrackingContext Initiate(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext trackingContext, string processingStepName);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep.Initiate(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,string).trackingContext'></a>

`trackingContext` [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')

The tracking context that is applicable just before entering the new processing step.

<a name='Be.Stateless.BizTalk.Activity.Tracking.Processing.ProcessingStep.Initiate(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,string).processingStepName'></a>

`processingStepName` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name of the processing step entered.

#### Returns
[TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')  
The new [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') for the processing step scope.