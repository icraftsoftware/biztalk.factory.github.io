#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Extensions](Be.Stateless.Extensions.md 'Be.Stateless.Extensions').[StringExtensions](StringExtensions.md 'Be.Stateless.Extensions.StringExtensions')

## StringExtensions.IfNotNullOrWhiteSpace(this string, Action<string>) Method

Performs an [System.Action&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1') delegate on the [string](StringExtensions.IfNotNullOrWhiteSpace(thisstring,Action_string_).md#Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace(thisstring,System.Action_string_).string 'Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace(this string, System.Action<string>).string') if it is not null or white space.

```csharp
public static void IfNotNullOrWhiteSpace(this string @string, System.Action<string> action);
```
#### Parameters

<a name='Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace(thisstring,System.Action_string_).string'></a>

`string` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string to test and to pass as argument to the [action](StringExtensions.IfNotNullOrWhiteSpace(thisstring,Action_string_).md#Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace(thisstring,System.Action_string_).action 'Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace(this string, System.Action<string>).action') delegate.

<a name='Be.Stateless.Extensions.StringExtensions.IfNotNullOrWhiteSpace(thisstring,System.Action_string_).action'></a>

`action` [System.Action&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')

The [System.Action&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1') delegate to perform.