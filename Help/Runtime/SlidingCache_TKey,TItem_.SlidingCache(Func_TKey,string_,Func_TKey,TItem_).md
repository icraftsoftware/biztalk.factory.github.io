#### [Be.Stateless.Runtime](README.md 'README')
### [Be.Stateless.Runtime.Caching](Be.Stateless.Runtime.Caching.md 'Be.Stateless.Runtime.Caching').[SlidingCache&lt;TKey,TItem&gt;](SlidingCache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>')

## SlidingCache(Func<TKey,string>, Func<TKey,TItem>) Constructor

Create the [Cache&lt;TKey,TItem&gt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>')-derived instance with a default sliding expiration of 30 minutes.

```csharp
protected SlidingCache(System.Func<TKey,string> keyFactory, System.Func<TKey,TItem> itemFactory);
```
#### Parameters

<a name='Be.Stateless.Runtime.Caching.SlidingCache_TKey,TItem_.SlidingCache(System.Func_TKey,string_,System.Func_TKey,TItem_).keyFactory'></a>

`keyFactory` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[TKey](SlidingCache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.SlidingCache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>.TKey')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')

Converts a [TKey](SlidingCache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.SlidingCache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>.TKey') item key to its string representation.

<a name='Be.Stateless.Runtime.Caching.SlidingCache_TKey,TItem_.SlidingCache(System.Func_TKey,string_,System.Func_TKey,TItem_).itemFactory'></a>

`itemFactory` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[TKey](SlidingCache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.SlidingCache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>.TKey')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[TItem](SlidingCache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.SlidingCache_TKey,TItem_.TItem 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>.TItem')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')

Returns the item to be added to the cache.