#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Text.Extensions](Be.Stateless.Text.Extensions.md 'Be.Stateless.Text.Extensions').[StringBuilderXmlExtensions](StringBuilderXmlExtensions.md 'Be.Stateless.Text.Extensions.StringBuilderXmlExtensions')

## StringBuilderXmlExtensions.GetReaderAtContent(this StringBuilder) Method

Returns an [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') over a [System.Text.StringBuilder](https://docs.microsoft.com/en-us/dotnet/api/System.Text.StringBuilder 'System.Text.StringBuilder') that contains XML data. Provided that the
content is not empty, the [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') will be positioned at the first content node.

```csharp
public static System.Xml.XmlReader GetReaderAtContent(this System.Text.StringBuilder builder);
```
#### Parameters

<a name='Be.Stateless.Text.Extensions.StringBuilderXmlExtensions.GetReaderAtContent(thisSystem.Text.StringBuilder).builder'></a>

`builder` [System.Text.StringBuilder](https://docs.microsoft.com/en-us/dotnet/api/System.Text.StringBuilder 'System.Text.StringBuilder')

The [System.Text.StringBuilder](https://docs.microsoft.com/en-us/dotnet/api/System.Text.StringBuilder 'System.Text.StringBuilder') containing the XML data.

#### Returns
[System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')  
An [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') over the XML content of the [System.Text.StringBuilder](https://docs.microsoft.com/en-us/dotnet/api/System.Text.StringBuilder 'System.Text.StringBuilder').