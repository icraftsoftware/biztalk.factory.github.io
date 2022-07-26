#### [Be.Stateless.BizTalk.Transform.ExtensionObjects](README.md 'README')
### [Be.Stateless.BizTalk.Transform.ExtensionObjects](Be.Stateless.BizTalk.Transform.ExtensionObjects.md 'Be.Stateless.BizTalk.Transform.ExtensionObjects').[RegexFunctions](RegexFunctions.md 'Be.Stateless.BizTalk.Transform.ExtensionObjects.RegexFunctions')

## RegexFunctions.Replace(string, string, string) Method

In a specified input string, replaces all strings that match a specified regular expression with a specified
replacement string.

```csharp
public string Replace(string input, string pattern, string replacement);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Transform.ExtensionObjects.RegexFunctions.Replace(string,string,string).input'></a>

`input` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string to search for a match.

<a name='Be.Stateless.BizTalk.Transform.ExtensionObjects.RegexFunctions.Replace(string,string,string).pattern'></a>

`pattern` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The regular expression pattern to match.

<a name='Be.Stateless.BizTalk.Transform.ExtensionObjects.RegexFunctions.Replace(string,string,string).replacement'></a>

`replacement` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The replacement string.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
A new string that is identical to the input string, except that the replacement string takes the place of each matched
string. If pattern is not matched in the current instance, the method returns the current instance unchanged.

### See Also
- [System.Text.RegularExpressions.Regex.Replace(System.String,System.String,System.String)](https://docs.microsoft.com/en-us/dotnet/api/System.Text.RegularExpressions.Regex.Replace#System_Text_RegularExpressions_Regex_Replace_System_String,System_String,System_String_ 'System.Text.RegularExpressions.Regex.Replace(System.String,System.String,System.String)')