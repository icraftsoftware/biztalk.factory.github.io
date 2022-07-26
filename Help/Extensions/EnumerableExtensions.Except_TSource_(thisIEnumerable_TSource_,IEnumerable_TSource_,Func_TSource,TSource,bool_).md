#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Linq.Extensions](Be.Stateless.Linq.Extensions.md 'Be.Stateless.Linq.Extensions').[EnumerableExtensions](EnumerableExtensions.md 'Be.Stateless.Linq.Extensions.EnumerableExtensions')

## EnumerableExtensions.Except<TSource>(this IEnumerable<TSource>, IEnumerable<TSource>, Func<TSource,TSource,bool>) Method

Produces the set difference of two sequences by using the specified [comparer](EnumerableExtensions.Except_TSource_(thisIEnumerable_TSource_,IEnumerable_TSource_,Func_TSource,TSource,bool_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Except_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).comparer 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Except<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Collections.Generic.IEnumerable<TSource>, System.Func<TSource,TSource,bool>).comparer') to compare values.

```csharp
public static System.Collections.Generic.IEnumerable<TSource> Except<TSource>(this System.Collections.Generic.IEnumerable<TSource> first, System.Collections.Generic.IEnumerable<TSource> second, System.Func<TSource,TSource,bool> comparer);
```
#### Type parameters

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Except_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).TSource'></a>

`TSource`

The type of the elements of the input sequences.
#### Parameters

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Except_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).first'></a>

`first` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[TSource](EnumerableExtensions.Except_TSource_(thisIEnumerable_TSource_,IEnumerable_TSource_,Func_TSource,TSource,bool_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Except_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Except<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Collections.Generic.IEnumerable<TSource>, System.Func<TSource,TSource,bool>).TSource')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

An [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') whose elements that are not also in second will be returned.

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Except_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).second'></a>

`second` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[TSource](EnumerableExtensions.Except_TSource_(thisIEnumerable_TSource_,IEnumerable_TSource_,Func_TSource,TSource,bool_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Except_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Except<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Collections.Generic.IEnumerable<TSource>, System.Func<TSource,TSource,bool>).TSource')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

An [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') whose elements that also occur in the first sequence will cause those elements to be
removed from the returned sequence.

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Except_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).comparer'></a>

`comparer` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-3 'System.Func`3')[TSource](EnumerableExtensions.Except_TSource_(thisIEnumerable_TSource_,IEnumerable_TSource_,Func_TSource,TSource,bool_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Except_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Except<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Collections.Generic.IEnumerable<TSource>, System.Func<TSource,TSource,bool>).TSource')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-3 'System.Func`3')[TSource](EnumerableExtensions.Except_TSource_(thisIEnumerable_TSource_,IEnumerable_TSource_,Func_TSource,TSource,bool_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Except_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Except<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Collections.Generic.IEnumerable<TSource>, System.Func<TSource,TSource,bool>).TSource')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-3 'System.Func`3')[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-3 'System.Func`3')

A lambda to compare values for equality.

#### Returns
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[TSource](EnumerableExtensions.Except_TSource_(thisIEnumerable_TSource_,IEnumerable_TSource_,Func_TSource,TSource,bool_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Except_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,TSource,bool_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Except<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Collections.Generic.IEnumerable<TSource>, System.Func<TSource,TSource,bool>).TSource')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
A sequence that contains the set difference of the elements of two sequences.