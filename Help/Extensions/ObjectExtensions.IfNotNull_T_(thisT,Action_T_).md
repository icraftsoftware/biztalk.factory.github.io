#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Extensions](Be.Stateless.Extensions.md 'Be.Stateless.Extensions').[ObjectExtensions](ObjectExtensions.md 'Be.Stateless.Extensions.ObjectExtensions')

## ObjectExtensions.IfNotNull<T>(this T, Action<T>) Method

Performs a [System.Action&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1') delegate on the [object](ObjectExtensions.IfNotNull_T_(thisT,Action_T_).md#Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T_(thisT,System.Action_T_).object 'Be.Stateless.Extensions.ObjectExtensions.IfNotNull<T>(this T, System.Action<T>).object') if it is not null.

```csharp
public static void IfNotNull<T>(this T @object, System.Action<T> action)
    where T : class;
```
#### Type parameters

<a name='Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T_(thisT,System.Action_T_).T'></a>

`T`

The type of [object](ObjectExtensions.IfNotNull_T_(thisT,Action_T_).md#Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T_(thisT,System.Action_T_).object 'Be.Stateless.Extensions.ObjectExtensions.IfNotNull<T>(this T, System.Action<T>).object').
#### Parameters

<a name='Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T_(thisT,System.Action_T_).object'></a>

`object` [T](ObjectExtensions.IfNotNull_T_(thisT,Action_T_).md#Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T_(thisT,System.Action_T_).T 'Be.Stateless.Extensions.ObjectExtensions.IfNotNull<T>(this T, System.Action<T>).T')

The object to test and to pass as argument to the [action](ObjectExtensions.IfNotNull_T_(thisT,Action_T_).md#Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T_(thisT,System.Action_T_).action 'Be.Stateless.Extensions.ObjectExtensions.IfNotNull<T>(this T, System.Action<T>).action') delegate.

<a name='Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T_(thisT,System.Action_T_).action'></a>

`action` [System.Action&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')[T](ObjectExtensions.IfNotNull_T_(thisT,Action_T_).md#Be.Stateless.Extensions.ObjectExtensions.IfNotNull_T_(thisT,System.Action_T_).T 'Be.Stateless.Extensions.ObjectExtensions.IfNotNull<T>(this T, System.Action<T>).T')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')

The [System.Action&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1') delegate to perform.