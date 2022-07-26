#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Extensions](Be.Stateless.Extensions.md 'Be.Stateless.Extensions').[ObjectExtensions](ObjectExtensions.md 'Be.Stateless.Extensions.ObjectExtensions')

## ObjectExtensions.IfNotNull<T,TR>(this T, Func<T,TR>) Method

Performs a [System.Func&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1') delegate on the [object](ObjectExtensions.IfNotNull_T,TR_(thisT,Func_T,TR_).md#Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T,TR_(thisT,System.Func_T,TR_).object 'Be.Stateless.Extensions.ObjectExtensions.IfNotNull<T,TR>(this T, System.Func<T,TR>).object') if it is not null and returns
the [function](ObjectExtensions.IfNotNull_T,TR_(thisT,Func_T,TR_).md#Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T,TR_(thisT,System.Func_T,TR_).function 'Be.Stateless.Extensions.ObjectExtensions.IfNotNull<T,TR>(this T, System.Func<T,TR>).function') delegate value.

```csharp
public static TR IfNotNull<T,TR>(this T @object, System.Func<T,TR> function)
    where T : class;
```
#### Type parameters

<a name='Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T,TR_(thisT,System.Func_T,TR_).T'></a>

`T`

The type of [object](ObjectExtensions.IfNotNull_T,TR_(thisT,Func_T,TR_).md#Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T,TR_(thisT,System.Func_T,TR_).object 'Be.Stateless.Extensions.ObjectExtensions.IfNotNull<T,TR>(this T, System.Func<T,TR>).object').

<a name='Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T,TR_(thisT,System.Func_T,TR_).TR'></a>

`TR`

The return type of the [System.Func&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1') delegate.
#### Parameters

<a name='Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T,TR_(thisT,System.Func_T,TR_).object'></a>

`object` [T](ObjectExtensions.IfNotNull_T,TR_(thisT,Func_T,TR_).md#Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T,TR_(thisT,System.Func_T,TR_).T 'Be.Stateless.Extensions.ObjectExtensions.IfNotNull<T,TR>(this T, System.Func<T,TR>).T')

The object to test and to pass as argument to the [function](ObjectExtensions.IfNotNull_T,TR_(thisT,Func_T,TR_).md#Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T,TR_(thisT,System.Func_T,TR_).function 'Be.Stateless.Extensions.ObjectExtensions.IfNotNull<T,TR>(this T, System.Func<T,TR>).function') delegate.

<a name='Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T,TR_(thisT,System.Func_T,TR_).function'></a>

`function` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[T](ObjectExtensions.IfNotNull_T,TR_(thisT,Func_T,TR_).md#Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T,TR_(thisT,System.Func_T,TR_).T 'Be.Stateless.Extensions.ObjectExtensions.IfNotNull<T,TR>(this T, System.Func<T,TR>).T')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[TR](ObjectExtensions.IfNotNull_T,TR_(thisT,Func_T,TR_).md#Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T,TR_(thisT,System.Func_T,TR_).TR 'Be.Stateless.Extensions.ObjectExtensions.IfNotNull<T,TR>(this T, System.Func<T,TR>).TR')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')

The [System.Func&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1') delegate to perform.

#### Returns
[TR](ObjectExtensions.IfNotNull_T,TR_(thisT,Func_T,TR_).md#Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T,TR_(thisT,System.Func_T,TR_).TR 'Be.Stateless.Extensions.ObjectExtensions.IfNotNull<T,TR>(this T, System.Func<T,TR>).TR')  
The result of the [function](ObjectExtensions.IfNotNull_T,TR_(thisT,Func_T,TR_).md#Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T,TR_(thisT,System.Func_T,TR_).function 'Be.Stateless.Extensions.ObjectExtensions.IfNotNull<T,TR>(this T, System.Func<T,TR>).function') delegate, or `default(TR)` if the [object](ObjectExtensions.IfNotNull_T,TR_(thisT,Func_T,TR_).md#Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T,TR_(thisT,System.Func_T,TR_).object 'Be.Stateless.Extensions.ObjectExtensions.IfNotNull<T,TR>(this T, System.Func<T,TR>).object')
is null.