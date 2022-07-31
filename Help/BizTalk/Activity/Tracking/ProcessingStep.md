#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Messaging](Be.Stateless.BizTalk.Activity.Tracking.Messaging.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging')

## ProcessingStep Class

```csharp
public class ProcessingStep
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ProcessingStep

| Constructors | |
| :--- | :--- |
| [ProcessingStep(string, EventStream)](ProcessingStep.ProcessingStep(string,EventStream).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.ProcessingStep(string, Microsoft.BizTalk.Bam.EventObservation.EventStream)') | |

| Properties | |
| :--- | :--- |
| [ActivityId](ProcessingStep.ActivityId.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.ActivityId') | |
| [BeginTime](ProcessingStep.BeginTime.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.BeginTime') | |
| [EndTime](ProcessingStep.EndTime.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.EndTime') | |
| [ErrorDescription](ProcessingStep.ErrorDescription.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.ErrorDescription') | |
| [MachineName](ProcessingStep.MachineName.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.MachineName') | |
| [ProcessActivityID](ProcessingStep.ProcessActivityID.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.ProcessActivityID') | |
| [Status](ProcessingStep.Status.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.Status') | |
| [StepName](ProcessingStep.StepName.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.StepName') | |

| Methods | |
| :--- | :--- |
| [AddCustomReference(string, string, string, string)](ProcessingStep.AddCustomReference(string,string,string,string).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.AddCustomReference(string, string, string, string)') | Add a custom reference to this activity, this enables 'data' to be attached to an activity, such as a message body. |
| [AddCustomReference(string, string, string)](ProcessingStep.AddCustomReference(string,string,string).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.AddCustomReference(string, string, string)') | Add a custom reference to this activity, this enables 'data' to be attached to an activity, such as a message body. |
| [AddReferenceToAnotherActivity(string, string)](ProcessingStep.AddReferenceToAnotherActivity(string,string).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.AddReferenceToAnotherActivity(string, string)') | Add a reference from this activity to another activity. |
| [BeginProcessingStepActivity()](ProcessingStep.BeginProcessingStepActivity().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.BeginProcessingStepActivity()') | Begins the BAM activity. |
| [CommitProcessingStepActivity()](ProcessingStep.CommitProcessingStepActivity().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.CommitProcessingStepActivity()') | Write any data changes to the BAM activity. This must be called after any property changes. |
| [EnableContinuation()](ProcessingStep.EnableContinuation().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.EnableContinuation()') | Activate continuation for this activity. While in the context that is enabling continuation, this activity can still be updated and MUST be ended with a call to EndProcessingStepActivity(). |
| [EndProcessingStepActivity()](ProcessingStep.EndProcessingStepActivity().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.EndProcessingStepActivity()') | End the BAM activity. No more changes will be permitted to this activity except by continuation. |
| [Flush()](ProcessingStep.Flush().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.Flush()') | Flush any buffered events. |
