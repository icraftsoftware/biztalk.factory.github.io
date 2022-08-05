#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Messaging](Be.Stateless.BizTalk.Activity.Tracking.Messaging.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging')

## ProcessMessagingStep Class

```csharp
public class ProcessMessagingStep
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ProcessMessagingStep

| Constructors | |
| :--- | :--- |
| [ProcessMessagingStep(string, EventStream)](ProcessMessagingStep.ProcessMessagingStep(string,EventStream).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessMessagingStep.ProcessMessagingStep(string, Microsoft.BizTalk.Bam.EventObservation.EventStream)') | |

| Properties | |
| :--- | :--- |
| [ActivityId](ProcessMessagingStep.ActivityId.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessMessagingStep.ActivityId') | |
| [MessagingStepActivityID](ProcessMessagingStep.MessagingStepActivityID.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessMessagingStep.MessagingStepActivityID') | |
| [MessagingStepStatus](ProcessMessagingStep.MessagingStepStatus.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessMessagingStep.MessagingStepStatus') | |
| [ProcessActivityID](ProcessMessagingStep.ProcessActivityID.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessMessagingStep.ProcessActivityID') | |

| Methods | |
| :--- | :--- |
| [AddCustomReference(string, string, string, string)](ProcessMessagingStep.AddCustomReference(string,string,string,string).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessMessagingStep.AddCustomReference(string, string, string, string)') | Add a custom reference to this activity, this enables 'data' to be attached to an activity, such as a message body. |
| [AddCustomReference(string, string, string)](ProcessMessagingStep.AddCustomReference(string,string,string).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessMessagingStep.AddCustomReference(string, string, string)') | Add a custom reference to this activity, this enables 'data' to be attached to an activity, such as a message body. |
| [AddReferenceToAnotherActivity(string, string)](ProcessMessagingStep.AddReferenceToAnotherActivity(string,string).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessMessagingStep.AddReferenceToAnotherActivity(string, string)') | Add a reference from this activity to another activity. |
| [BeginProcessMessagingStepActivity()](ProcessMessagingStep.BeginProcessMessagingStepActivity().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessMessagingStep.BeginProcessMessagingStepActivity()') | Begins the BAM activity. |
| [CommitProcessMessagingStepActivity()](ProcessMessagingStep.CommitProcessMessagingStepActivity().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessMessagingStep.CommitProcessMessagingStepActivity()') | Write any data changes to the BAM activity. This must be called after any property changes. |
| [EnableContinuation()](ProcessMessagingStep.EnableContinuation().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessMessagingStep.EnableContinuation()') | Activate continuation for this activity. While in the context that is enabling continuation, this activity can still be updated and MUST be ended with a call to EndProcessMessagingStepActivity(). |
| [EndProcessMessagingStepActivity()](ProcessMessagingStep.EndProcessMessagingStepActivity().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessMessagingStep.EndProcessMessagingStepActivity()') | End the BAM activity. No more changes will be permitted to this activity except by continuation. |
| [Flush()](ProcessMessagingStep.Flush().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessMessagingStep.Flush()') | Flush any buffered events. |
