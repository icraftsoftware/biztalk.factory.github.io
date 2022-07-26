#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Extensions](Be.Stateless.Extensions.md 'Be.Stateless.Extensions').[StringXmlExtensions](StringXmlExtensions.md 'Be.Stateless.Extensions.StringXmlExtensions')

## StringXmlExtensions.TryParseQName(this string, string, string) Method

Try to parse a qualified name and extracts its prefix and local parts.

```csharp
public static bool TryParseQName(this string qName, out string prefix, out string localPart);
```
#### Parameters

<a name='Be.Stateless.Extensions.StringXmlExtensions.TryParseQName(thisstring,string,string).qName'></a>

`qName` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The qualified to parse.

<a name='Be.Stateless.Extensions.StringXmlExtensions.TryParseQName(thisstring,string,string).prefix'></a>

`prefix` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The prefix part of the qName if it is a valid qualified name; [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty') if there is no prefix part.

<a name='Be.Stateless.Extensions.StringXmlExtensions.TryParseQName(thisstring,string,string).localPart'></a>

`localPart` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The local part of the qName if it is a valid qualified name.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if it is a valid qualified name; `false` otherwise.

### See Also
- [Qualified Names](http://www.w3.org/TR/xml-names/#ns-qualnames 'http://www.w3.org/TR/xml-names/#ns-qualnames')