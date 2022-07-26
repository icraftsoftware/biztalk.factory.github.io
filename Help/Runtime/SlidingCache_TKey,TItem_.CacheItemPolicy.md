#### [Be.Stateless.Runtime](README.md 'README')
### [Be.Stateless.Runtime.Caching](Be.Stateless.Runtime.Caching.md 'Be.Stateless.Runtime.Caching').[SlidingCache&lt;TKey,TItem&gt;](SlidingCache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>')

## SlidingCache<TKey,TItem>.CacheItemPolicy Property

Returns a sliding expiration [CacheItemPolicy](SlidingCache_TKey,TItem_.CacheItemPolicy.md 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>.CacheItemPolicy') according to the [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan') provided at
construction time of this [SlidingCache&lt;TKey,TItem&gt;](SlidingCache_TKey,TItem_.md 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>') object.

```csharp
protected override System.Runtime.Caching.CacheItemPolicy CacheItemPolicy { get; }
```

#### Property Value
[System.Runtime.Caching.CacheItemPolicy](https://docs.microsoft.com/en-us/dotnet/api/System.Runtime.Caching.CacheItemPolicy 'System.Runtime.Caching.CacheItemPolicy')

### Remarks
The sliding expiration defaults to 30 minutes, unless specified otherwise via the [SlidingCache(Func&lt;TKey,string&gt;, Func&lt;TKey,TItem&gt;, TimeSpan)](SlidingCache_TKey,TItem_.SlidingCache(Func_TKey,string_,Func_TKey,TItem_,TimeSpan).md 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>.SlidingCache(System.Func<TKey,string>, System.Func<TKey,TItem>, System.TimeSpan)') constructor.

### See Also
- [SlidingCache(Func&lt;TKey,string&gt;, Func&lt;TKey,TItem&gt;)](SlidingCache_TKey,TItem_.SlidingCache(Func_TKey,string_,Func_TKey,TItem_).md 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>.SlidingCache(System.Func<TKey,string>, System.Func<TKey,TItem>)')
- [SlidingCache(Func&lt;TKey,string&gt;, Func&lt;TKey,TItem&gt;, TimeSpan)](SlidingCache_TKey,TItem_.SlidingCache(Func_TKey,string_,Func_TKey,TItem_,TimeSpan).md 'Be.Stateless.Runtime.Caching.SlidingCache<TKey,TItem>.SlidingCache(System.Func<TKey,string>, System.Func<TKey,TItem>, System.TimeSpan)')