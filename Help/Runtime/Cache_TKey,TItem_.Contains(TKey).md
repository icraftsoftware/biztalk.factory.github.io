#### [Be.Stateless.Runtime](README.md 'README')
### [Be.Stateless.Runtime.Caching](Be.Stateless.Runtime.Caching.md 'Be.Stateless.Runtime.Caching').[Cache&lt;TKey,TItem&gt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>')

## Cache<TKey,TItem>.Contains(TKey) Method

Determines whether a cache entry exists in the cache for the [TKey](Cache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.TKey') instance.

```csharp
public bool Contains(TKey key);
```
#### Parameters

<a name='Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.Contains(TKey).key'></a>

`key` [TKey](Cache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.TKey')

The [TKey](Cache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.TKey') instance to search for in cache.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if the cache contains an entry for the [TKey](Cache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.TKey') instance; otherwise, `false`.