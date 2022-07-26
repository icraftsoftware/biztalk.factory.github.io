#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Extensions](Be.Stateless.Extensions.md 'Be.Stateless.Extensions').[StringExtensions](StringExtensions.md 'Be.Stateless.Extensions.StringExtensions')

## StringExtensions.IsNullOrWhiteSpace(this string) Method

Indicates whether a specified string is null, empty, or consists only of white-space characters.

```csharp
public static bool IsNullOrWhiteSpace(this string @string);
```
#### Parameters

<a name='Be.Stateless.Extensions.StringExtensions.IsNullOrWhiteSpace(thisstring).string'></a>

`string` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string to test.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if the [string](StringExtensions.IsNullOrWhiteSpace(thisstring).md#Be.Stateless.Extensions.StringExtensions.IsNullOrWhiteSpace(thisstring).string 'Be.Stateless.Extensions.StringExtensions.IsNullOrWhiteSpace(this string).string') argument is null or an [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty'), or if it
            consists exclusively of white-space characters; otherwise `false`.