#### [Be.Stateless.Runtime](README.md 'README')
### [Be.Stateless.Runtime.Caching](Be.Stateless.Runtime.Caching.md 'Be.Stateless.Runtime.Caching')

## SlidingCache<TKey,TItem> Class

Simple runtime memory cache base class with sliding expiration <seealso cref="P:Be.Stateless.Runtime.Caching.SlidingCache`2.CacheItemPolicy"/>.

```csharp
public abstract class SlidingCache<TKey,TItem> : Be.Stateless.Runtime.Caching.Cache<TKey, TItem>
```
#### Type parameters

<a name='Be.Stateless.Runtime.Caching.SlidingCache_TKey,TItem_.TKey'></a>

`TKey`

The type of the objects to be used as key.

<a name='Be.Stateless.Runtime.Caching.SlidingCache_TKey,TItem_.TItem'></a>

`TItem`

The type of the objects to be cached.

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.Runtime.Caching.Cache&lt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>')[TKey](SlidingCache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.SlidingCache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>.TKey')[,](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>')[TItem](SlidingCache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.SlidingCache_TKey,TItem_.TItem 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>.TItem')[&gt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>') &#129106; SlidingCache<TKey,TItem>

### Remarks
This cache attaches a sliding expiration <seealso cref="P:Be.Stateless.Runtime.Caching.SlidingCache`2.CacheItemPolicy"/> to each item it adds to the [System.Runtime.Caching.MemoryCache](https://docs.microsoft.com/en-us/dotnet/api/System.Runtime.Caching.MemoryCache 'System.Runtime.Caching.MemoryCache') that is created behind the scene.

### See Also
- [Cache&lt;TKey,TItem&gt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>')
- [System.Runtime.Caching.MemoryCache](https://docs.microsoft.com/en-us/dotnet/api/System.Runtime.Caching.MemoryCache 'System.Runtime.Caching.MemoryCache')

| Constructors | |
| :--- | :--- |
| [SlidingCache(Func&lt;TKey,string&gt;, Func&lt;TKey,TItem&gt;, TimeSpan)](SlidingCache_TKey,TItem_.SlidingCache(Func_TKey,string_,Func_TKey,TItem_,TimeSpan).md 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>.SlidingCache(System.Func<TKey,string>, System.Func<TKey,TItem>, System.TimeSpan)') | Create the [Cache&lt;TKey,TItem&gt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>')-derived instance and overrides the default sliding expiration. |
| [SlidingCache(Func&lt;TKey,string&gt;, Func&lt;TKey,TItem&gt;)](SlidingCache_TKey,TItem_.SlidingCache(Func_TKey,string_,Func_TKey,TItem_).md 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>.SlidingCache(System.Func<TKey,string>, System.Func<TKey,TItem>)') | Create the [Cache&lt;TKey,TItem&gt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>')-derived instance with a default sliding expiration of 30 minutes. |

| Properties | |
| :--- | :--- |
| [CacheItemPolicy](SlidingCache_TKey,TItem_.CacheItemPolicy.md 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>.CacheItemPolicy') | Returns a sliding expiration [CacheItemPolicy](SlidingCache_TKey,TItem_.CacheItemPolicy.md 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>.CacheItemPolicy') according to the [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan') provided at construction time of this [SlidingCache&lt;TKey,TItem&gt;](SlidingCache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>') object. |
