#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking](Be.Stateless.BizTalk.Activity.Tracking.md 'Be.Stateless.BizTalk.Activity.Tracking').[ActivityId](ActivityId.md 'Be.Stateless.BizTalk.Activity.Tracking.ActivityId')

## ActivityId.AsNormalizedActivityId(this string) Method

Normalize the string activity id to have a homogenous [System.Guid](https://docs.microsoft.com/en-us/dotnet/api/System.Guid 'System.Guid') format across all BAM tracking activities.

```csharp
public static string AsNormalizedActivityId(this string id);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.ActivityId.AsNormalizedActivityId(thisstring).id'></a>

`id` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string [System.Guid](https://docs.microsoft.com/en-us/dotnet/api/System.Guid 'System.Guid') to normalize.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
The normalized string activity id.