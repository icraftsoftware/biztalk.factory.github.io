#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Linq.Extensions](Be.Stateless.Linq.Extensions.md 'Be.Stateless.Linq.Extensions').[EnumerableExtensions](EnumerableExtensions.md 'Be.Stateless.Linq.Extensions.EnumerableExtensions')

## EnumerableExtensions.Single<TSource>(this IEnumerable<TSource>, Func<Exception>, Func<Exception>) Method

Returns the only element of a sequence, and throws an exception if there is not exactly one element in the sequence.

```csharp
public static TSource Single<TSource>(this System.Collections.Generic.IEnumerable<TSource> source, System.Func<System.Exception> noElementExceptionFactory, System.Func<System.Exception> moreThanOneElementExceptionFactory);
```
#### Type parameters

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Single_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_System.Exception_,System.Func_System.Exception_).TSource'></a>

`TSource`
#### Parameters

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Single_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_System.Exception_,System.Func_System.Exception_).source'></a>

`source` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[TSource](EnumerableExtensions.Single_TSource_(thisIEnumerable_TSource_,Func_Exception_,Func_Exception_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Single_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_System.Exception_,System.Func_System.Exception_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Single<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Func<System.Exception>, System.Func<System.Exception>).TSource')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

An [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') to return the single element of.

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Single_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_System.Exception_,System.Func_System.Exception_).noElementExceptionFactory'></a>

`noElementExceptionFactory` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1')[System.Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Exception 'System.Exception')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1')

The exception to throw if the input sequence contains no element.

<a name='Be.Stateless.Linq.Extensions.EnumerableExtensions.Single_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_System.Exception_,System.Func_System.Exception_).moreThanOneElementExceptionFactory'></a>

`moreThanOneElementExceptionFactory` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1')[System.Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Exception 'System.Exception')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1')

The exception to throw if the input sequence contains more than one element.

#### Returns
[TSource](EnumerableExtensions.Single_TSource_(thisIEnumerable_TSource_,Func_Exception_,Func_Exception_).md#Be.Stateless.Linq.Extensions.EnumerableExtensions.Single_TSource_(thisSystem.Collections.Generic.IEnumerable_TSource_,System.Func_System.Exception_,System.Func_System.Exception_).TSource 'Be.Stateless.Linq.Extensions.EnumerableExtensions.Single<TSource>(this System.Collections.Generic.IEnumerable<TSource>, System.Func<System.Exception>, System.Func<System.Exception>).TSource')  
The single element of the input sequence.