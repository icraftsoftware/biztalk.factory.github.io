#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Extensions](Be.Stateless.Extensions.md 'Be.Stateless.Extensions').[StringExtensions](StringExtensions.md 'Be.Stateless.Extensions.StringExtensions')

## StringExtensions.SubstringEx(this string, int) Method

Extract the first or last `length` characters of a string, whether `length` is respectively positive
or negative.

```csharp
public static string SubstringEx(this string @string, int length);
```
#### Parameters

<a name='Be.Stateless.Extensions.StringExtensions.SubstringEx(thisstring,int).string'></a>

`string` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string to extract characters of.

<a name='Be.Stateless.Extensions.StringExtensions.SubstringEx(thisstring,int).length'></a>

`length` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The number of characters to extract.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
The substring of the input string.

### Remarks
Returns an empty string if the input string is null or empty. If the length of the input string is less than
`length`, the whole string is returned.