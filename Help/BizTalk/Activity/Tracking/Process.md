#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Messaging](Be.Stateless.BizTalk.Activity.Tracking.Messaging.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging')

## Process Class

Allows to track activity of a process at the messaging level.

```csharp
public class Process
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; Process

| Constructors | |
| :--- | :--- |
| [Process(IPipelineContext, IBaseMessage)](Process.Process(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.Process(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
| [Process(string, EventStream)](Process.Process(string,EventStream).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.Process(string, Microsoft.BizTalk.Bam.EventObservation.EventStream)') | |

| Properties | |
| :--- | :--- |
| [ActivityId](Process.ActivityId.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.ActivityId') | |
| [BeginTime](Process.BeginTime.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.BeginTime') | |
| [EndTime](Process.EndTime.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.EndTime') | |
| [EventStream](Process.EventStream.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.EventStream') | |
| [InterchangeID](Process.InterchangeID.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.InterchangeID') | |
| [ProcessName](Process.ProcessName.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.ProcessName') | |
| [Status](Process.Status.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.Status') | |
| [Value1](Process.Value1.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.Value1') | |
| [Value2](Process.Value2.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.Value2') | |
| [Value3](Process.Value3.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.Value3') | |

| Methods | |
| :--- | :--- |
| [AddCustomReference(string, string, string, string)](Process.AddCustomReference(string,string,string,string).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.AddCustomReference(string, string, string, string)') | Add a custom reference to this activity, this enables 'data' to be attached to an activity, such as a message body. |
| [AddCustomReference(string, string, string)](Process.AddCustomReference(string,string,string).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.AddCustomReference(string, string, string)') | Add a custom reference to this activity, this enables 'data' to be attached to an activity, such as a message body. |
| [AddReferenceToAnotherActivity(string, string)](Process.AddReferenceToAnotherActivity(string,string).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.AddReferenceToAnotherActivity(string, string)') | Add a reference from this activity to another activity. |
| [AddStep(MessagingStep)](Process.AddStep(MessagingStep).md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.AddStep(Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep)') | |
| [BeginProcessActivity()](Process.BeginProcessActivity().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.BeginProcessActivity()') | Begins the BAM activity. |
| [CommitProcessActivity()](Process.CommitProcessActivity().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.CommitProcessActivity()') | Write any data changes to the BAM activity. This must be called after any property changes. |
| [EnableContinuation()](Process.EnableContinuation().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.EnableContinuation()') | Activate continuation for this activity. While in the context that is enabling continuation, this activity can still be updated and MUST be ended with a call to EndProcessActivity(). |
| [EndProcessActivity()](Process.EndProcessActivity().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.EndProcessActivity()') | End the BAM activity. No more changes will be permitted to this activity except by continuation. |
| [Flush()](Process.Flush().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.Flush()') | Flush any buffered events. |
| [TrackActivity()](Process.TrackActivity().md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process.TrackActivity()') | |
