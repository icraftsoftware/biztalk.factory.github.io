#### [Be.Stateless.Runtime](README.md 'README')
### [Be.Stateless.Runtime.Caching](Be.Stateless.Runtime.Caching.md 'Be.Stateless.Runtime.Caching')

## Cache<TKey,TItem> Class

Simple runtime memory cache base class.

```csharp
public abstract class Cache<TKey,TItem>
```
#### Type parameters

<a name='Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.TKey'></a>

`TKey`

The type of the objects to be used as key.

<a name='Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.TItem'></a>

`TItem`

The type of the objects to be cached.

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; Cache<TKey,TItem>

Derived  
&#8627; [AbsoluteCache&lt;TKey,TItem&gt;](AbsoluteCache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>')  
&#8627; [SlidingCache&lt;TKey,TItem&gt;](SlidingCache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>')

### Remarks
For each derived class, [Cache&lt;TKey,TItem&gt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>') creates behind the scene a named memory cache instance, i.e. a
[System.Runtime.Caching.MemoryCache](https://docs.microsoft.com/en-us/dotnet/api/System.Runtime.Caching.MemoryCache 'System.Runtime.Caching.MemoryCache'), named after the most-derived class name.

| Constructors | |
| :--- | :--- |
| [Cache(Func&lt;TKey,string&gt;, Func&lt;TKey,TItem&gt;)](Cache_TKey,TItem_.Cache(Func_TKey,string_,Func_TKey,TItem_).md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.Cache(System.Func<TKey,string>, System.Func<TKey,TItem>)') | Create the [Cache&lt;TKey,TItem&gt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>')-derived instance. |

| Properties | |
| :--- | :--- |
| [CacheItemPolicy](Cache_TKey,TItem_.CacheItemPolicy.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.CacheItemPolicy') | [CacheItemPolicy](Cache_TKey,TItem_.CacheItemPolicy.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.CacheItemPolicy') to be used for any new item that will be added to the cache. |
| [this[TKey]](Cache_TKey,TItem_.this[TKey].md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.this[TKey]') | Gets, and sets if not already in cache, the [TItem](Cache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.TItem 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.TItem') instance associated to the [TKey](Cache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.TKey') instance. |

| Methods | |
| :--- | :--- |
| [Contains(TKey)](Cache_TKey,TItem_.Contains(TKey).md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.Contains(TKey)') | Determines whether a cache entry exists in the cache for the [TKey](Cache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.Cache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>.TKey') instance. |
