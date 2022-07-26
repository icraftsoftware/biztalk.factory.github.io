#### [Be.Stateless.Runtime](README.md 'README')
### [Be.Stateless.Runtime.Caching](Be.Stateless.Runtime.Caching.md 'Be.Stateless.Runtime.Caching').[AbsoluteCache&lt;TKey,TItem&gt;](AbsoluteCache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>')

## AbsoluteCache(Func<TKey,string>, Func<TKey,TItem>, TimeSpan) Constructor

Create the [Cache&lt;TKey,TItem&gt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>')-derived instance and overrides the default absolute expiration.

```csharp
protected AbsoluteCache(System.Func<TKey,string> keyFactory, System.Func<TKey,TItem> itemFactory, System.TimeSpan absoluteExpirationDuration);
```
#### Parameters

<a name='Be.Stateless.Runtime.Caching.AbsoluteCache_TKey,TItem_.AbsoluteCache(System.Func_TKey,string_,System.Func_TKey,TItem_,System.TimeSpan).keyFactory'></a>

`keyFactory` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[TKey](AbsoluteCache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.AbsoluteCache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>.TKey')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')

Converts a [TKey](AbsoluteCache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.AbsoluteCache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>.TKey') item key to its string representation.

<a name='Be.Stateless.Runtime.Caching.AbsoluteCache_TKey,TItem_.AbsoluteCache(System.Func_TKey,string_,System.Func_TKey,TItem_,System.TimeSpan).itemFactory'></a>

`itemFactory` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[TKey](AbsoluteCache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.AbsoluteCache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>.TKey')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[TItem](AbsoluteCache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.AbsoluteCache_TKey,TItem_.TItem 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>.TItem')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')

Returns the item to be added to the cache.

<a name='Be.Stateless.Runtime.Caching.AbsoluteCache_TKey,TItem_.AbsoluteCache(System.Func_TKey,string_,System.Func_TKey,TItem_,System.TimeSpan).absoluteExpirationDuration'></a>

`absoluteExpirationDuration` [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

The [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan') denoting the absolute expiration duration from the time an item was is to the cache.