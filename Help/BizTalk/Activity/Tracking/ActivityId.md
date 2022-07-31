#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking](Be.Stateless.BizTalk.Activity.Tracking.md 'Be.Stateless.BizTalk.Activity.Tracking')

## ActivityId Class

Helper class that offers a central and unique place to generate homogenous and normalized BAM activity ids.

```csharp
public static class ActivityId
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ActivityId

| Methods | |
| :--- | :--- |
| [AsNormalizedActivityId(this string)](ActivityId.AsNormalizedActivityId(thisstring).md 'Be.Stateless.BizTalk.Activity.Tracking.ActivityId.AsNormalizedActivityId(this string)') | Normalize the string activity id to have a homogenous [System.Guid](https://docs.microsoft.com/en-us/dotnet/api/System.Guid 'System.Guid') format across all BAM tracking activities. |
| [AsNormalizedActivityId(this Guid)](ActivityId.AsNormalizedActivityId(thisGuid).md 'Be.Stateless.BizTalk.Activity.Tracking.ActivityId.AsNormalizedActivityId(this System.Guid)') | Convert [System.Guid](https://docs.microsoft.com/en-us/dotnet/api/System.Guid 'System.Guid') to a normalized string activity id. |
| [NewActivityId()](ActivityId.NewActivityId().md 'Be.Stateless.BizTalk.Activity.Tracking.ActivityId.NewActivityId()') | Generate a new tracking activity id as a normalized string activity id. |
