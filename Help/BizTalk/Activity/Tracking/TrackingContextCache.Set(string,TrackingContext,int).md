#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Runtime.Caching](Be.Stateless.BizTalk.Runtime.Caching.md 'Be.Stateless.BizTalk.Runtime.Caching').[TrackingContextCache](TrackingContextCache.md 'Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache')

## TrackingContextCache.Set(string, TrackingContext, int) Method

Adds a new or update an existing [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') in cache with an absolute expiration of [duration](TrackingContextCache.Set(string,TrackingContext,int).md#Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Set(string,Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,int).duration 'Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Set(string, Be.Stateless.BizTalk.Activity.Tracking.TrackingContext, int).duration').

```csharp
public virtual void Set(string key, Be.Stateless.BizTalk.Activity.Tracking.TrackingContext trackingContext, int duration);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Set(string,Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,int).key'></a>

`key` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The cache entry identifier, or key, at which to add the new [trackingContext](TrackingContextCache.Set(string,TrackingContext,int).md#Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Set(string,Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,int).trackingContext 'Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Set(string, Be.Stateless.BizTalk.Activity.Tracking.TrackingContext, int).trackingContext').

<a name='Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Set(string,Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,int).trackingContext'></a>

`trackingContext` [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')

The [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') to cache.

<a name='Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Set(string,Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,int).duration'></a>

`duration` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The duration, in seconds, after which the [trackingContext](TrackingContextCache.Set(string,TrackingContext,int).md#Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Set(string,Be.Stateless.BizTalk.Activity.Tracking.TrackingContext,int).trackingContext 'Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Set(string, Be.Stateless.BizTalk.Activity.Tracking.TrackingContext, int).trackingContext') entry will be removed from the cache.