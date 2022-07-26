#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml.Extensions](Be.Stateless.Xml.Extensions.md 'Be.Stateless.Xml.Extensions').[XmlReaderExtensions](XmlReaderExtensions.md 'Be.Stateless.Xml.Extensions.XmlReaderExtensions')

## XmlReaderExtensions.IsEndElement(this XmlReader, string, string) Method

Tests if the current content node is an end tag whose [System.Xml.XmlReader.LocalName](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.LocalName 'System.Xml.XmlReader.LocalName') and [System.Xml.XmlReader.NamespaceURI](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.NamespaceURI 'System.Xml.XmlReader.NamespaceURI') properties match the given [name](XmlReaderExtensions.IsEndElement(thisXmlReader,string,string).md#Be.Stateless.Xml.Extensions.XmlReaderExtensions.IsEndElement(thisSystem.Xml.XmlReader,string,string).name 'Be.Stateless.Xml.Extensions.XmlReaderExtensions.IsEndElement(this System.Xml.XmlReader, string, string).name') and [ns](XmlReaderExtensions.IsEndElement(thisXmlReader,string,string).md#Be.Stateless.Xml.Extensions.XmlReaderExtensions.IsEndElement(thisSystem.Xml.XmlReader,string,string).ns 'Be.Stateless.Xml.Extensions.XmlReaderExtensions.IsEndElement(this System.Xml.XmlReader, string, string).ns')
arguments.

```csharp
public static bool IsEndElement(this System.Xml.XmlReader reader, string name, string ns);
```
#### Parameters

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.IsEndElement(thisSystem.Xml.XmlReader,string,string).reader'></a>

`reader` [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')

An [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') object.

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.IsEndElement(thisSystem.Xml.XmlReader,string,string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string to match against the [System.Xml.XmlReader.LocalName](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.LocalName 'System.Xml.XmlReader.LocalName') property of the element found.

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.IsEndElement(thisSystem.Xml.XmlReader,string,string).ns'></a>

`ns` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string to match against the [System.Xml.XmlReader.NamespaceURI](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.NamespaceURI 'System.Xml.XmlReader.NamespaceURI') property of the element found.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')