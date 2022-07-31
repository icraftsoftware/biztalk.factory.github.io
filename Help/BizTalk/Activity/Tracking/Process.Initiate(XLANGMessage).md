#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Processing](Be.Stateless.BizTalk.Activity.Tracking.Processing.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing').[Process](Process.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process')

## Process.Initiate(XLANGMessage) Method

Method intended to be called at the start of an orchestration to create a BAM process tracking activity.

```csharp
public static Be.Stateless.BizTalk.Activity.Tracking.TrackingContext Initiate(Microsoft.XLANGs.BaseTypes.XLANGMessage activatingMessage);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.Initiate(Microsoft.XLANGs.BaseTypes.XLANGMessage).activatingMessage'></a>

`activatingMessage` [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')

The message that activates the orchestration instance.

#### Returns
[TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')  
The [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') that contains the BAM tracking activities identifiers for the current process.
Notice that [TrackingContext.MessagingStepActivityId](TrackingContext.MessagingStepActivityId.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext.MessagingStepActivityId') will be
filled with the tracking activity identifier of [activatingMessage](Process.Initiate(XLANGMessage).md#Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.Initiate(Microsoft.XLANGs.BaseTypes.XLANGMessage).activatingMessage 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.Initiate(Microsoft.XLANGs.BaseTypes.XLANGMessage).activatingMessage') if it exists.

### Remarks
The name used for the process instance is automatically determined by the ambient message context property [TrackingProperties.ProcessName](TrackingProperties.ProcessName.md 'Be.Stateless.BizTalk.ContextProperties.TrackingProperties.ProcessName') should it be non null nor empty, or the
containing namespace of the calling orchestration otherwise.