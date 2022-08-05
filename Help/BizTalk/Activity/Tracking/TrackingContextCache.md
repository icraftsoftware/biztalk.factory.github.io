#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Runtime.Caching](Be.Stateless.BizTalk.Runtime.Caching.md 'Be.Stateless.BizTalk.Runtime.Caching')

## TrackingContextCache Class

Runtime memory cache for the [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') associated to [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage')-derived types.

```csharp
public class TrackingContextCache
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; TrackingContextCache

| Properties | |
| :--- | :--- |
| [Instance](TrackingContextCache.Instance.md 'Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Instance') | |

| Methods | |
| :--- | :--- |
| [Get(string)](TrackingContextCache.Get(string).md 'Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Get(string)') | Returns a previously cached [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext'). |
| [Remove(string)](TrackingContextCache.Remove(string).md 'Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Remove(string)') | Removes and returns a previously cached [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext'). |
| [Set(string, TrackingContext, int)](TrackingContextCache.Set(string,TrackingContext,int).md 'Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Set(string, Be.Stateless.BizTalk.Activity.Tracking.TrackingContext, int)') | Adds a new or update an existing [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') in cache with an absolute expiration of [duration](TrackingContextCache.Set(string,TrackingContext,int).md#Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Set(string,Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,int).duration 'Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Set(string, Be.Stateless.BizTalk.Activity.Tracking.TrackingContext, int).duration'). |
