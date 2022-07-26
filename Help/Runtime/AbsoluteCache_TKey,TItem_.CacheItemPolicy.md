#### [Be.Stateless.Runtime](README.md 'README')
### [Be.Stateless.Runtime.Caching](Be.Stateless.Runtime.Caching.md 'Be.Stateless.Runtime.Caching').[AbsoluteCache&lt;TKey,TItem&gt;](AbsoluteCache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>')

## AbsoluteCache<TKey,TItem>.CacheItemPolicy Property

Returns an absolute expiration [CacheItemPolicy](AbsoluteCache_TKey,TItem_.CacheItemPolicy.md 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>.CacheItemPolicy') according to the duration provided by the [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan') given at construction time of this [AbsoluteCache&lt;TKey,TItem&gt;](AbsoluteCache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>') object.

```csharp
protected override System.Runtime.Caching.CacheItemPolicy CacheItemPolicy { get; }
```

#### Property Value
[System.Runtime.Caching.CacheItemPolicy](https://docs.microsoft.com/en-us/dotnet/api/System.Runtime.Caching.CacheItemPolicy 'System.Runtime.Caching.CacheItemPolicy')

### Remarks
The absolute expiration duration defaults to 30 minutes, unless specified otherwise via the [AbsoluteCache(Func&lt;TKey,string&gt;, Func&lt;TKey,TItem&gt;, TimeSpan)](AbsoluteCache_TKey,TItem_.AbsoluteCache(Func_TKey,string_,Func_TKey,TItem_,TimeSpan).md 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>.AbsoluteCache(System.Func<TKey,string>, System.Func<TKey,TItem>, System.TimeSpan)') constructor.

### See Also
- [AbsoluteCache(Func&lt;TKey,string&gt;, Func&lt;TKey,TItem&gt;)](AbsoluteCache_TKey,TItem_.AbsoluteCache(Func_TKey,string_,Func_TKey,TItem_).md 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>.AbsoluteCache(System.Func<TKey,string>, System.Func<TKey,TItem>)')
- [AbsoluteCache(Func&lt;TKey,string&gt;, Func&lt;TKey,TItem&gt;, TimeSpan)](AbsoluteCache_TKey,TItem_.AbsoluteCache(Func_TKey,string_,Func_TKey,TItem_,TimeSpan).md 'Be.Stateless.Runtime.Caching.AbsoluteCache<TKey,TItem>.AbsoluteCache(System.Func<TKey,string>, System.Func<TKey,TItem>, System.TimeSpan)')