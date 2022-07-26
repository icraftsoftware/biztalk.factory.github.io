#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Linq.Extensions](Be.Stateless.Linq.Extensions.md 'Be.Stateless.Linq.Extensions').[EnumerableExtensions](EnumerableExtensions.md 'Be.Stateless.Linq.Extensions.EnumerableExtensions')

## EnumerableExtensions.Distinct<TSource>(this IEnumerable<TSource>, Func<TSource,TSource,bool>) Method

Returns distinct elements from a sequence by using a specified [comparer](EnumerableExtensions.Distinct_TSource_(thisIEnumerable_TSource_,Func_TSource,TSource,bool_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Distinct_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).comparer 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Distinct<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Func<TSource,TSource,bool>).comparer') to compare values.

```csharp
public static System.Collections.Generic.IEnumerable<TSource> Distinct<TSource>(this System.Collections.Generic.IEnumerable<TSource> source, System.Func<TSource,TSource,bool> comparer);
```
#### Type parameters

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Distinct_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).TSource'></a>

`TSource`

The type of the elements of source.
#### Parameters

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Distinct_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).source'></a>

`source` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[TSource](EnumerableExtensions.Distinct_TSource_(thisIEnumerable_TSource_,Func_TSource,TSource,bool_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Distinct_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Distinct<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Func<TSource,TSource,bool>).TSource')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

The sequence to remove duplicate elements from.

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Distinct_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).comparer'></a>

`comparer` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-3 'System.Func`3')[TSource](EnumerableExtensions.Distinct_TSource_(thisIEnumerable_TSource_,Func_TSource,TSource,bool_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Distinct_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Distinct<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Func<TSource,TSource,bool>).TSource')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-3 'System.Func`3')[TSource](EnumerableExtensions.Distinct_TSource_(thisIEnumerable_TSource_,Func_TSource,TSource,bool_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Distinct_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Distinct<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Func<TSource,TSource,bool>).TSource')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-3 'System.Func`3')[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-3 'System.Func`3')

A lambda to compare values for equality.

#### Returns
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[TSource](EnumerableExtensions.Distinct_TSource_(thisIEnumerable_TSource_,Func_TSource,TSource,bool_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Distinct_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Distinct<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Func<TSource,TSource,bool>).TSource')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
An [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') that contains distinct elements from the source sequence.