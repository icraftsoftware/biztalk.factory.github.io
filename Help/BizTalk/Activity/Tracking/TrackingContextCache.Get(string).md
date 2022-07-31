#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Runtime.Caching](Be.Stateless.BizTalk.Runtime.Caching.md 'Be.Stateless.BizTalk.Runtime.Caching').[TrackingContextCache](TrackingContextCache.md 'Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache')

## TrackingContextCache.Get(string) Method

Returns a previously cached [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext').

```csharp
public virtual Be.Stateless.BizTalk.Activity.Tracking.TrackingContext Get(string key);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Get(string).key'></a>

`key` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The cache entry identifier, or key, of the [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') to retrieve.

#### Returns
[TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')  
The [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') that had been previously added to the cache.

#### Exceptions

[System.ArgumentNullException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentNullException 'System.ArgumentNullException')  
The key is null or empty.

[System.InvalidOperationException](https://docs.microsoft.com/en-us/dotnet/api/System.InvalidOperationException 'System.InvalidOperationException')  
No entry has been found in cache for the given [key](TrackingContextCache.Get(string).md#Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Get(string).key 'Be.Stateless.BizTalk.Runtime.Caching.TrackingContextCache.Get(string).key'), or the [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') is
invalid.