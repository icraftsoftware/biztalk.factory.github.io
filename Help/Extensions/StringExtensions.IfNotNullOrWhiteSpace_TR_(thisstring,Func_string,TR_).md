#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Extensions](Be.Stateless.Extensions.md 'Be.Stateless.Extensions').[StringExtensions](StringExtensions.md 'Be.Stateless.Extensions.StringExtensions')

## StringExtensions.IfNotNullOrWhiteSpace<TR>(this string, Func<string,TR>) Method

Performs an [System.Func&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1') delegate on the [string](StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,Func_string,TR_).md#Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,System.Func_string,TR_).string 'Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace<TR>(this string, System.Func<string,TR>).string') if it is not null or white space
and returns the [function](StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,Func_string,TR_).md#Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,System.Func_string,TR_).function 'Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace<TR>(this string, System.Func<string,TR>).function') delegate value.

```csharp
public static TR IfNotNullOrWhiteSpace<TR>(this string @string, System.Func<string,TR> function);
```
#### Type parameters

<a name='Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,System.Func_string,TR_).TR'></a>

`TR`

The return type of the [System.Func&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1') delegate.
#### Parameters

<a name='Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,System.Func_string,TR_).string'></a>

`string` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string to test and to pass as argument to the [function](StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,Func_string,TR_).md#Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,System.Func_string,TR_).function 'Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace<TR>(this string, System.Func<string,TR>).function') delegate.

<a name='Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,System.Func_string,TR_).function'></a>

`function` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[TR](StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,Func_string,TR_).md#Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,System.Func_string,TR_).TR 'Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace<TR>(this string, System.Func<string,TR>).TR')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')

The [System.Func&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1') delegate to perform.

#### Returns
[TR](StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,Func_string,TR_).md#Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,System.Func_string,TR_).TR 'Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace<TR>(this string, System.Func<string,TR>).TR')  
The result of the [function](StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,Func_string,TR_).md#Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,System.Func_string,TR_).function 'Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace<TR>(this string, System.Func<string,TR>).function') delegate, or `default(TR)` if the [string](StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,Func_string,TR_).md#Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace_TR_(thisstring,System.Func_string,TR_).string 'Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace<TR>(this string, System.Func<string,TR>).string') is
null or white space.