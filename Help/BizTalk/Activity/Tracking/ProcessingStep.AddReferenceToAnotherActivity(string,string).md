#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Messaging](Be.Stateless.BizTalk.Activity.Tracking.Messaging.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging').[ProcessingStep](ProcessingStep.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep')

## ProcessingStep.AddReferenceToAnotherActivity(string, string) Method

Add a reference from this activity to another activity.

```csharp
public void AddReferenceToAnotherActivity(string otherActivityName, string otherActivityId);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.AddReferenceToAnotherActivity(string,string).otherActivityName'></a>

`otherActivityName` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The related activity name. Reference names are limited to 128 characters.

<a name='Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep.AddReferenceToAnotherActivity(string,string).otherActivityId'></a>

`otherActivityId` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The related activity Id. Limited to 1024 characters of data.