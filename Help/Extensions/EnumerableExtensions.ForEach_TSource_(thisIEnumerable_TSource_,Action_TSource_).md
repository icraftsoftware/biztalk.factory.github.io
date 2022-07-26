#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Linq.Extensions](Be.Stateless.Linq.Extensions.md 'Be.Stateless.Linq.Extensions').[EnumerableExtensions](EnumerableExtensions.md 'Be.Stateless.Linq.Extensions.EnumerableExtensions')

## EnumerableExtensions.ForEach<TSource>(this IEnumerable<TSource>, Action<TSource>) Method

Calls an [System.Action&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1') delegate for each element of a sequence.

```csharp
public static void ForEach<TSource>(this System.Collections.Generic.IEnumerable<TSource> source, System.Action<TSource> action);
```
#### Type parameters

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.ForEach_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Action_TSource_).TSource'></a>

`TSource`

The type of the elements of [source](EnumerableExtensions.ForEach_TSource_(thisIEnumerable_TSource_,Action_TSource_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.ForEach_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Action_TSource_).source 'Be.Stateless.Linq.Extensions.EnumerableExtensions.ForEach<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Action<TSource>).source').
#### Parameters

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.ForEach_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Action_TSource_).source'></a>

`source` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[TSource](EnumerableExtensions.ForEach_TSource_(thisIEnumerable_TSource_,Action_TSource_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.ForEach_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Action_TSource_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.ForEach<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Action<TSource>).TSource')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

A sequence of values to invoke an action delegate on.

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.ForEach_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Action_TSource_).action'></a>

`action` [System.Action&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')[TSource](EnumerableExtensions.ForEach_TSource_(thisIEnumerable_TSource_,Action_TSource_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.ForEach_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Action_TSource_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.ForEach<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Action<TSource>).TSource')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')

An [System.Action&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1') delegate to apply to each element.