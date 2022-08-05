#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Processing](Be.Stateless.BizTalk.Activity.Tracking.Processing.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing').[Process](Process.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process')

## Process.Initiate(XLANGMessage, string) Method

Method intended to be called at the start of an orchestration to create a BAM process tracking activity.

```csharp
public static Be.Stateless.BizTalk.Activity.Tracking.TrackingContext Initiate(Microsoft.XLANGs.BaseTypes.XLANGMessage activatingMessage, string processName);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.Initiate(Microsoft.XLANGs.BaseTypes.XLANGMessage,string).activatingMessage'></a>

`activatingMessage` [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')

The message that activates the orchestration instance.

<a name='Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.Initiate(Microsoft.XLANGs.BaseTypes.XLANGMessage,string).processName'></a>

`processName` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name that will be used to qualify the new tracked process instance.

#### Returns
[TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')  
The [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') that contains the BAM tracking activities identifiers for the current process.
Notice that [MessagingStepActivityId](TrackingContext.MessagingStepActivityId.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext.MessagingStepActivityId') will be filled with the tracking activity
identifier of [activatingMessage](Process.Initiate(XLANGMessage,string).md#Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.Initiate(Microsoft.XLANGs.BaseTypes.XLANGMessage,string).activatingMessage 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.Initiate(Microsoft.XLANGs.BaseTypes.XLANGMessage, string).activatingMessage') if it exists.