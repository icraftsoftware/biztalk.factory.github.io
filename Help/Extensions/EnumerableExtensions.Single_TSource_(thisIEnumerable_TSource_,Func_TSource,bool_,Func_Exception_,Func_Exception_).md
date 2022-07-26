#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Linq.Extensions](Be.Stateless.Linq.Extensions.md 'Be.Stateless.Linq.Extensions').[EnumerableExtensions](EnumerableExtensions.md 'Be.Stateless.Linq.Extensions.EnumerableExtensions')

## EnumerableExtensions.Single<TSource>(this IEnumerable<TSource>, Func<TSource,bool>, Func<Exception>, Func<Exception>) Method

Returns the only element of a sequence that satisfies a specified condition, and throws an exception if more than one
such element exists.

```csharp
public static TSource Single<TSource>(this System.Collections.Generic.IEnumerable<TSource> source, System.Func<TSource,bool> predicate, System.Func<System.Exception> noElementExceptionFactory, System.Func<System.Exception> moreThanOneElementExceptionFactory);
```
#### Type parameters

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Single_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,bool_,System.Func_System.Exception_,System.Func_System.Exception_).TSource'></a>

`TSource`

A function to test an element for a condition.
#### Parameters

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Single_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,bool_,System.Func_System.Exception_,System.Func_System.Exception_).source'></a>

`source` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[TSource](EnumerableExtensions.Single_TSource_(thisIEnumerable_TSource_,Func_TSource,bool_,Func_Exception_,Func_Exception_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Single_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,bool_,System.Func_System.Exception_,System.Func_System.Exception_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Single<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Func<TSource,bool>, System.Func<System.Exception>, System.Func<System.Exception>).TSource')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

An [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') to return the single element of.

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Single_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,bool_,System.Func_System.Exception_,System.Func_System.Exception_).predicate'></a>

`predicate` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[TSource](EnumerableExtensions.Single_TSource_(thisIEnumerable_TSource_,Func_TSource,bool_,Func_Exception_,Func_Exception_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Single_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,bool_,System.Func_System.Exception_,System.Func_System.Exception_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Single<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Func<TSource,bool>, System.Func<System.Exception>, System.Func<System.Exception>).TSource')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')

A function to test an element for a condition.

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Single_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,bool_,System.Func_System.Exception_,System.Func_System.Exception_).noElementExceptionFactory'></a>

`noElementExceptionFactory` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1')[System.Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Exception 'System.Exception')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1')

The exception to throw if the input sequence contains no element that satisfies the condition.

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Single_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,bool_,System.Func_System.Exception_,System.Func_System.Exception_).moreThanOneElementExceptionFactory'></a>

`moreThanOneElementExceptionFactory` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1')[System.Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Exception 'System.Exception')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1')

The exception to throw if the input sequence contains more than one element that satisfies the condition.

#### Returns
[TSource](EnumerableExtensions.Single_TSource_(thisIEnumerable_TSource_,Func_TSource,bool_,Func_Exception_,Func_Exception_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Single_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_TSource,bool_,System.Func_System.Exception_,System.Func_System.Exception_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Single<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Func<TSource,bool>, System.Func<System.Exception>, System.Func<System.Exception>).TSource')  
The single element of the input sequence that satisfies a condition.