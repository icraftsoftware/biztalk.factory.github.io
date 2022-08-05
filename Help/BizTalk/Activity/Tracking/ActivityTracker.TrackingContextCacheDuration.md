#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent').[ActivityTracker](ActivityTracker.md 'Be.Stateless.BizTalk.MicroComponent.ActivityTracker')

## ActivityTracker.TrackingContextCacheDuration Property

How long activity tracking contexts will be kept in cache when propagated through solicit-response ports. Any
negative value disables caching.

```csharp
public System.TimeSpan TrackingContextCacheDuration { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')