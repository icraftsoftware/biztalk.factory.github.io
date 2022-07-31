#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Messaging](Be.Stateless.BizTalk.Activity.Tracking.Messaging.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging').[IActivityFactory](IActivityFactory.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.IActivityFactory')

## IActivityFactory.FindMessagingStep(TrackingContext) Method

Creates a [Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStepReference](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStepReference 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStepReference') tracking activity denoting an already tracked message.

```csharp
Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep FindMessagingStep(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext trackingContext);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Messaging.IActivityFactory.FindMessagingStep(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext).trackingContext'></a>

`trackingContext` [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')

The [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') whose [MessagingStepActivityId](TrackingContext.MessagingStepActivityId.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext.MessagingStepActivityId') identifies the already
tracked [MessagingStep](MessagingStep.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep').

#### Returns
[MessagingStep](MessagingStep.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep')  
A [Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStepReference](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStepReference 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStepReference') instance that will be used to feed the BAM Process activity: specifically,
affiliating it to a [Process](Process.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process') tracking activity.