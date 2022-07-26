#### [Be.Stateless.Runtime](README.md 'README')
### [Be.Stateless.Runtime.Caching](Be.Stateless.Runtime.Caching.md 'Be.Stateless.Runtime.Caching').[Cache&lt;TKey,TItem&gt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>')

## Cache<TKey,TItem>.this[TKey] Property

Gets, and sets if not already in cache, the [TItem](Cache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.TItem 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.TItem') instance associated to the [TKey](Cache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.TKey') instance.

```csharp
public TItem this[TKey key] { get; }
```
#### Parameters

<a name='Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.this[TKey].key'></a>

`key` [TKey](Cache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.TKey')

The [TKey](Cache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.TKey') key object instance to get or set in cache.

#### Property Value
[TItem](Cache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.TItem 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.TItem')

### Remarks
When the cache does not already contain the [TItem](Cache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.TItem 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.TItem') instance, it is inserted into the cache with
[CacheItemPolicy](Cache_TKey,TItem_.CacheItemPolicy.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.CacheItemPolicy') provided by the derived class.