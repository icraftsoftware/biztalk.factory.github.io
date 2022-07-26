#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml.Extensions](Be.Stateless.Xml.Extensions.md 'Be.Stateless.Xml.Extensions').[XmlReaderExtensions](XmlReaderExtensions.md 'Be.Stateless.Xml.Extensions.XmlReaderExtensions')

## XmlReaderExtensions.IsEndElement(this XmlReader, string) Method

Tests if the current content node is an end tag whose [System.Xml.XmlReader.Name](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.Name 'System.Xml.XmlReader.Name') matches the given [name](XmlReaderExtensions.IsEndElement(thisXmlReader,string).md#Be.Stateless.Xml.Extensions.XmlReaderExtensions.IsEndElement(thisSystem.Xml.XmlReader,string).name 'Be.Stateless.Xml.Extensions.XmlReaderExtensions.IsEndElement(this System.Xml.XmlReader, string).name') argument.

```csharp
public static bool IsEndElement(this System.Xml.XmlReader reader, string name);
```
#### Parameters

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.IsEndElement(thisSystem.Xml.XmlReader,string).reader'></a>

`reader` [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')

An [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') object.

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.IsEndElement(thisSystem.Xml.XmlReader,string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string to match against the [System.Xml.XmlReader.Name](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.Name 'System.Xml.XmlReader.Name') property of the element found.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')