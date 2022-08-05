#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Messaging](Be.Stateless.BizTalk.Activity.Tracking.Messaging.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging').[MessagingStep](MessagingStep.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep')

## MessagingStep.AddCustomReference(string, string, string) Method

Add a custom reference to this activity, this enables 'data' to be attached to an activity, such as a message body.

```csharp
public void AddCustomReference(string referenceType, string referenceName, string referenceData);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.AddCustomReference(string,string,string).referenceType'></a>

`referenceType` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The related item type. Reference type identifiers are limited to 128 characters.

<a name='Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.AddCustomReference(string,string,string).referenceName'></a>

`referenceName` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The related item name. Reference names are limited to 128 characters.

<a name='Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep.AddCustomReference(string,string,string).referenceData'></a>

`referenceData` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The related item data. Limited to 1024 characters of data.