#### [Be.Stateless.BizTalk.Transform.ExtensionObjects](README.md 'README')
### [Be.Stateless.BizTalk.Transform.ExtensionObjects](Be.Stateless.BizTalk.Transform.ExtensionObjects.md 'Be.Stateless.BizTalk.Transform.ExtensionObjects').[RegexFunctions](RegexFunctions.md 'Be.Stateless.BizTalk.Transform.ExtensionObjects.RegexFunctions')

## RegexFunctions.IsMatch(string, string) Method

Indicates whether the specified regular expression finds a match in the specified input string.

```csharp
public bool IsMatch(string input, string pattern);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Transform.ExtensionObjects.RegexFunctions.IsMatch(string,string).input'></a>

`input` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string to search for a match.

<a name='Be.Stateless.BizTalk.Transform.ExtensionObjects.RegexFunctions.IsMatch(string,string).pattern'></a>

`pattern` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The regular expression pattern to match.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if the regular expression finds a match; `false` otherwise.

### See Also
- [System.Text.RegularExpressions.Regex.IsMatch(System.String,System.String)](https://docs.microsoft.com/en-us/dotnet/api/System.Text.RegularExpressions.Regex.IsMatch#System_Text_RegularExpressions_Regex_IsMatch_System_String,System_String_ 'System.Text.RegularExpressions.Regex.IsMatch(System.String,System.String)')