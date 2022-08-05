#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Processing](Be.Stateless.BizTalk.Activity.Tracking.Processing.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing').[Process](Process.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process')

## Process.AddStep(TrackingContext, XLANGMessage) Method

Adds a messaging step to a process.

```csharp
public static void AddStep(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext trackingContext, Microsoft.XLANGs.BaseTypes.XLANGMessage message);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.AddStep(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,Microsoft.XLANGs.BaseTypes.XLANGMessage).trackingContext'></a>

`trackingContext` [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')

The [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') that contains the [ProcessActivityId](TrackingContext.ProcessActivityId.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext.ProcessActivityId') of the process
tracking activity.

<a name='Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.AddStep(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,Microsoft.XLANGs.BaseTypes.XLANGMessage).message'></a>

`message` [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')

The message whose BAM tracking activity must be attached to the process tracking activity.

### Remarks
It is typically used when an orchestration receives a message in the middle of its execution, or when convoys are
used to start it. In these cases, the message(s) cannot be associated with the process in the receive pipeline, and a
call to this method is needed. Notice that to attach a single activating message to a process, the [Initiate(XLANGMessage)](Process.Initiate(XLANGMessage).md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.Initiate(Microsoft.XLANGs.BaseTypes.XLANGMessage)') method must be used instead.