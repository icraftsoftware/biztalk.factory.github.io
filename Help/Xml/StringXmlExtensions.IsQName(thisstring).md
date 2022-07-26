#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Extensions](Be.Stateless.Extensions.md 'Be.Stateless.Extensions').[StringXmlExtensions](StringXmlExtensions.md 'Be.Stateless.Extensions.StringXmlExtensions')

## StringXmlExtensions.IsQName(this string) Method

Verifies that the [qName](StringXmlExtensions.IsQName(thisstring).md#Be.Stateless.Extensions.StringXmlExtensions.IsQName(thisstring).qName 'Be.Stateless.Extensions.StringXmlExtensions.IsQName(this string).qName') string is a valid qualified name according to the W3C Extended Markup
Language recommendation.

```csharp
public static bool IsQName(this string qName);
```
#### Parameters

<a name='Be.Stateless.Extensions.StringXmlExtensions.IsQName(thisstring).qName'></a>

`qName` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The QName to verify.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if it is a valid qualified name; `false` otherwise.

### See Also
- [http://www.w3.org/TR/2009/REC-xml-names-20091208/#ns-qualnames](http://www.w3.org/TR/2009/REC-xml-names-20091208/#ns-qualnames 'http://www.w3.org/TR/2009/REC-xml-names-20091208/#ns-qualnames')