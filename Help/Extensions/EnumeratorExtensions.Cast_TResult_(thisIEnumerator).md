#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Linq.Extensions](Be.Stateless.Linq.Extensions.md 'Be.Stateless.Linq.Extensions').[EnumeratorExtensions](EnumeratorExtensions.md 'Be.Stateless.Linq.Extensions.EnumeratorExtensions')

## EnumeratorExtensions.Cast<TResult>(this IEnumerator) Method

Casts the elements of an [System.Collections.IEnumerator](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.IEnumerator 'System.Collections.IEnumerator') to the specified type.

```csharp
public static System.Collections.Generic.IEnumerable<TResult> Cast<TResult>(this System.Collections.IEnumerator source);
```
#### Type parameters

<a name='Be.Stateless.Linq.Extensions.EnumeratorExtensions.Cast_TResult_(thisSystem.Collections.IEnumerator).TResult'></a>

`TResult`

The type to cast the elements of source to.
#### Parameters

<a name='Be.Stateless.Linq.Extensions.EnumeratorExtensions.Cast_TResult_(thisSystem.Collections.IEnumerator).source'></a>

`source` [System.Collections.IEnumerator](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.IEnumerator 'System.Collections.IEnumerator')

The [System.Collections.IEnumerator](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.IEnumerator 'System.Collections.IEnumerator') that contains the elements to be cast to type [TResult](EnumeratorExtensions.Cast_TResult_(thisIEnumerator).md#Be.Stateless.Linq.Extensions.EnumeratorExtensions.Cast_TResult_(thisSystem.Collections.IEnumerator).TResult 'Be.Stateless.Linq.Extensions.EnumeratorExtensions.Cast<TResult>(this System.Collections.IEnumerator).TResult').

#### Returns
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[TResult](EnumeratorExtensions.Cast_TResult_(thisIEnumerator).md#Be.Stateless.Linq.Extensions.EnumeratorExtensions.Cast_TResult_(thisSystem.Collections.IEnumerator).TResult 'Be.Stateless.Linq.Extensions.EnumeratorExtensions.Cast<TResult>(this System.Collections.IEnumerator).TResult')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
An [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') that contains each element of the [source](EnumeratorExtensions.Cast_TResult_(thisIEnumerator).md#Be.Stateless.Linq.Extensions.EnumeratorExtensions.Cast_TResult_(thisSystem.Collections.IEnumerator).source 'Be.Stateless.Linq.Extensions.EnumeratorExtensions.Cast<TResult>(this System.Collections.IEnumerator).source') sequence cast to the
specified type.