#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Extensions](Be.Stateless.Extensions.md 'Be.Stateless.Extensions').[StringExtensions](StringExtensions.md 'Be.Stateless.Extensions.StringExtensions')

## StringExtensions.Parse<T>(this string, bool) Method

Converts the string representation of the name or numeric value of one or more enumerated constants to an
equivalent enumerated object.

```csharp
public static T Parse<T>(this string value, bool ignoreCase=true)
    where T : struct, System.ValueType, System.ValueType;
```
#### Type parameters

<a name='Be.Stateless.Extensions.StringExtensions.Parse_T_(thisstring,bool).T'></a>

`T`

An enumeration type.
#### Parameters

<a name='Be.Stateless.Extensions.StringExtensions.Parse_T_(thisstring,bool).value'></a>

`value` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

A string containing the name or value to convert.

<a name='Be.Stateless.Extensions.StringExtensions.Parse_T_(thisstring,bool).ignoreCase'></a>

`ignoreCase` [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

Whether to ignore case or not; `true` by default.

#### Returns
[T](StringExtensions.Parse_T_(thisstring,bool).md#Be.Stateless.Extensions.StringExtensions.Parse_T_(thisstring,bool).T 'Be.Stateless.Extensions.StringExtensions.Parse<T>(this string, bool).T')  
One or more enumerated constants of type [T](StringExtensions.Parse_T_(thisstring,bool).md#Be.Stateless.Extensions.StringExtensions.Parse_T_(thisstring,bool).T 'Be.Stateless.Extensions.StringExtensions.Parse<T>(this string, bool).T') that represents [value](StringExtensions.Parse_T_(thisstring,bool).md#Be.Stateless.Extensions.StringExtensions.Parse_T_(thisstring,bool).value 'Be.Stateless.Extensions.StringExtensions.Parse<T>(this string, bool).value').