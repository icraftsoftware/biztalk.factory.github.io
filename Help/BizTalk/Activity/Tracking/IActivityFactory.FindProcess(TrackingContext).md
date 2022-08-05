#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Messaging](Be.Stateless.BizTalk.Activity.Tracking.Messaging.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging').[IActivityFactory](IActivityFactory.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.IActivityFactory')

## IActivityFactory.FindProcess(TrackingContext) Method

Creates a [Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessReference](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessReference 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessReference') tracking activity denoting an already tracked, though possibly ongoing,
process.

```csharp
Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process FindProcess(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext trackingContext);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Messaging.IActivityFactory.FindProcess(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext).trackingContext'></a>

`trackingContext` [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')

The [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') whose [ProcessActivityId](TrackingContext.ProcessActivityId.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext.ProcessActivityId') identifies the ongoing
process.

#### Returns
[Process](Process.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process')  
A [Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessReference](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessReference 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessReference') instance that will be used to feed the BAM Process activity: specifically,
affiliating new [MessagingStep](MessagingStep.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep') tracking activities.