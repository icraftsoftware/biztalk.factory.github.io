#### [Be.Stateless.Runtime](README.md 'README')
### [Be.Stateless.Runtime.Caching](Be.Stateless.Runtime.Caching.md 'Be.Stateless.Runtime.Caching')

## AbsoluteCache<TKey,TItem> Class

Simple runtime memory cache base class with absolute expiration <seealso cref="P:Be.Stateless.Runtime.Caching.AbsoluteCache`2.CacheItemPolicy"/>.

```csharp
public abstract class AbsoluteCache<TKey,TItem> : Be.Stateless.Runtime.Caching.Cache<TKey, TItem>
```
#### Type parameters

<a name='Be.Stateless.Runtime.Caching.AbsoluteCache_TKey,TItem_.TKey'></a>

`TKey`

The type of the objects to be used as key.

<a name='Be.Stateless.Runtime.Caching.AbsoluteCache_TKey,TItem_.TItem'></a>

`TItem`

The type of the objects to be cached.

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.Runtime.Caching.Cache&lt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>')[TKey](AbsoluteCache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.AbsoluteCache_TKey,TItem_.TKey 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>.TKey')[,](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>')[TItem](AbsoluteCache_TKey,TItem_.md#Be.Stateless.Runtime.Caching.AbsoluteCache_TKey,TItem_.TItem 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>.TItem')[&gt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>') &#129106; AbsoluteCache<TKey,TItem>

### Remarks
This cache attaches an absolute expiration <seealso cref="P:Be.Stateless.Runtime.Caching.AbsoluteCache`2.CacheItemPolicy"/> to each item it adds to the [System.Runtime.Caching.MemoryCache](https://docs.microsoft.com/en-us/dotnet/api/System.Runtime.Caching.MemoryCache 'System.Runtime.Caching.MemoryCache') that is created behind the scene.

### See Also
- [Cache&lt;TKey,TItem&gt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>')
- [System.Runtime.Caching.MemoryCache](https://docs.microsoft.com/en-us/dotnet/api/System.Runtime.Caching.MemoryCache 'System.Runtime.Caching.MemoryCache')

| Constructors | |
| :--- | :--- |
| [AbsoluteCache(Func&lt;TKey,string&gt;, Func&lt;TKey,TItem&gt;, TimeSpan)](AbsoluteCache_TKey,TItem_.AbsoluteCache(Func_TKey,string_,Func_TKey,TItem_,TimeSpan).md 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>.AbsoluteCache(System.Func<TKey,string>, System.Func<TKey,TItem>, System.TimeSpan)') | Create the [Cache&lt;TKey,TItem&gt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>')-derived instance and overrides the default absolute expiration. |
| [AbsoluteCache(Func&lt;TKey,string&gt;, Func&lt;TKey,TItem&gt;)](AbsoluteCache_TKey,TItem_.AbsoluteCache(Func_TKey,string_,Func_TKey,TItem_).md 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>.AbsoluteCache(System.Func<TKey,string>, System.Func<TKey,TItem>)') | Create the [Cache&lt;TKey,TItem&gt;](Cache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.Cache<TKey,TItem>')-derived instance with a default absolute expiration of 30 minutes from the time the item is added to the cache. |

| Properties | |
| :--- | :--- |
| [CacheItemPolicy](AbsoluteCache_TKey,TItem_.CacheItemPolicy.md 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>.CacheItemPolicy') | Returns an absolute expiration [CacheItemPolicy](AbsoluteCache_TKey,TItem_.CacheItemPolicy.md 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>.CacheItemPolicy') according to the duration provided by the [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan') given at construction time of this [AbsoluteCache&lt;TKey,TItem&gt;](AbsoluteCache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>') object. |
