#### [Be.Stateless.BizTalk.Transform.ExtensionObjects](README.md 'README')
### [Be.Stateless.BizTalk.Transform.ExtensionObjects](Be.Stateless.BizTalk.Transform.ExtensionObjects.md 'Be.Stateless.BizTalk.Transform.ExtensionObjects').[XmlConversionFunctions](XmlConversionFunctions.md 'Be.Stateless.BizTalk.Transform.ExtensionObjects.XmlConversionFunctions')

## XmlConversionFunctions.ToBoolean(string) Method

Converts the [string](XmlConversionFunctions.ToBoolean(string).md#Be.Stateless.BizTalk.Transform.ExtensionObjects.XmlConversionFunctions.ToBoolean(string).string 'Be.Stateless.BizTalk.Transform.ExtensionObjects.XmlConversionFunctions.ToBoolean(string).string') string to a Boolean equivalent.

```csharp
public bool ToBoolean(string @string);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Transform.ExtensionObjects.XmlConversionFunctions.ToBoolean(string).string'></a>

`string` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string to convert.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
A [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') value, that is `true` or `false`.

### Remarks

According to XML Schema Definition Language [boolean](https://www.w3.org/TR/xmlschema11-2/#boolean 'https://www.w3.org/TR/xmlschema11-2/#boolean'), a
boolean can have either of the following values: `'true'`, `'false'`, `'1'`, or `'0'`. Converting
a boolean literal to a boolean value therefore requires to write the following expression in XPath 1.0:
`<xsl:value-of select='boolean(number(text())) = true() or text() = 'true''/>`.

This function provides a shorter way of doing it: `<xsl:value-of select='xc:ToBoolean(text())'/>`,
assuming `xc` denotes the XML namespace referencing the extension object [XmlConversionFunctions](XmlConversionFunctions.md 'Be.Stateless.BizTalk.Transform.ExtensionObjects.XmlConversionFunctions').