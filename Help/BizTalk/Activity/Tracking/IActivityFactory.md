#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Messaging](Be.Stateless.BizTalk.Activity.Tracking.Messaging.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging')

## IActivityFactory Interface

Tracking-activity factory for messaging-only activities, i.e. [Microsoft.BizTalk.Bam.EventObservation.EventStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Bam.EventObservation.EventStream 'Microsoft.BizTalk.Bam.EventObservation.EventStream')-based activities.

```csharp
public interface IActivityFactory
```

Derived  
&#8627; [ActivityFactory](ActivityFactory.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ActivityFactory')

### Remarks
Notice that, as this is a messaging-only activity factory API, there is no way to create a [ProcessingStep](ProcessingStep.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep')
activity.

| Methods | |
| :--- | :--- |
| [CreateMessagingStep(IBaseMessage)](IActivityFactory.CreateMessagingStep(IBaseMessage).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.IActivityFactory.CreateMessagingStep(Microsoft.BizTalk.Message.Interop.IBaseMessage)') | Creates a [MessagingStep](MessagingStep.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep') tracking activity denoting a message yet to be tracked. |
| [CreateProcess(IBaseMessage, string)](IActivityFactory.CreateProcess(IBaseMessage,string).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.IActivityFactory.CreateProcess(Microsoft.BizTalk.Message.Interop.IBaseMessage, string)') | Creates a [Process](Process.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process') tracking activity denoting a process yet to be tracked. |
| [FindMessagingStep(TrackingContext)](IActivityFactory.FindMessagingStep(TrackingContext).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.IActivityFactory.FindMessagingStep(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext)') | Creates a [Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStepReference](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStepReference 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStepReference') tracking activity denoting an already tracked message. |
| [FindProcess(TrackingContext)](IActivityFactory.FindProcess(TrackingContext).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.IActivityFactory.FindProcess(Be.Stateless.BizTalk.Activity.Tracking.TrackingContext)') | Creates a [Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessReference](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessReference 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessReference') tracking activity denoting an already tracked, though possibly ongoing, process. |
