#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Messaging](Be.Stateless.BizTalk.Activity.Tracking.Messaging.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging')

## MessagingStep Class

Allows to track activity of a messaging step at the messaging level.

```csharp
public class MessagingStep
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; MessagingStep

| Constructors | |
| :--- | :--- |
| [MessagingStep(string, EventStream)](MessagingStep.MessagingStep(string,EventStream).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.MessagingStep(string, Microsoft.BizTalk.Bam.EventObservation.EventStream)') | |

| Properties | |
| :--- | :--- |
| [ActivityId](MessagingStep.ActivityId.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.ActivityId') | |
| [ErrorCode](MessagingStep.ErrorCode.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.ErrorCode') | |
| [ErrorDescription](MessagingStep.ErrorDescription.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.ErrorDescription') | |
| [InterchangeID](MessagingStep.InterchangeID.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.InterchangeID') | |
| [MachineName](MessagingStep.MachineName.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.MachineName') | |
| [Message](MessagingStep.Message.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.Message') | The actual [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage') message that this messaging step is all about. |
| [MessageID](MessagingStep.MessageID.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.MessageID') | |
| [MessageSize](MessagingStep.MessageSize.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.MessageSize') | |
| [MessageType](MessagingStep.MessageType.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.MessageType') | |
| [PortName](MessagingStep.PortName.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.PortName') | |
| [RetryCount](MessagingStep.RetryCount.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.RetryCount') | |
| [Status](MessagingStep.Status.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.Status') | |
| [Time](MessagingStep.Time.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.Time') | |
| [TransportLocation](MessagingStep.TransportLocation.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.TransportLocation') | |
| [TransportType](MessagingStep.TransportType.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.TransportType') | |
| [Value1](MessagingStep.Value1.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.Value1') | |
| [Value2](MessagingStep.Value2.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.Value2') | |
| [Value3](MessagingStep.Value3.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.Value3') | |

| Methods | |
| :--- | :--- |
| [AddCustomReference(string, string, string, string)](MessagingStep.AddCustomReference(string,string,string,string).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.AddCustomReference(string, string, string, string)') | Add a custom reference to this activity, this enables 'data' to be attached to an activity, such as a message body. |
| [AddCustomReference(string, string, string)](MessagingStep.AddCustomReference(string,string,string).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.AddCustomReference(string, string, string)') | Add a custom reference to this activity, this enables 'data' to be attached to an activity, such as a message body. |
| [AddReferenceToAnotherActivity(string, string)](MessagingStep.AddReferenceToAnotherActivity(string,string).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.AddReferenceToAnotherActivity(string, string)') | Add a reference from this activity to another activity. |
| [BeginMessagingStepActivity()](MessagingStep.BeginMessagingStepActivity().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.BeginMessagingStepActivity()') | Begins the BAM activity. |
| [CommitMessagingStepActivity()](MessagingStep.CommitMessagingStepActivity().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.CommitMessagingStepActivity()') | Write any data changes to the BAM activity. This must be called after any property changes. |
| [EnableContinuation()](MessagingStep.EnableContinuation().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.EnableContinuation()') | Activate continuation for this activity. While in the context that is enabling continuation, this activity can still be updated and MUST be ended with a call to EndMessagingStepActivity(). |
| [EndMessagingStepActivity()](MessagingStep.EndMessagingStepActivity().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.EndMessagingStepActivity()') | End the BAM activity. No more changes will be permitted to this activity except by continuation. |
| [Flush()](MessagingStep.Flush().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.Flush()') | Flush any buffered events. |
