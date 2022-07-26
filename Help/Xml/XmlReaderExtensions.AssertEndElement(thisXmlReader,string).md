#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml.Extensions](Be.Stateless.Xml.Extensions.md 'Be.Stateless.Xml.Extensions').[XmlReaderExtensions](XmlReaderExtensions.md 'Be.Stateless.Xml.Extensions.XmlReaderExtensions')

## XmlReaderExtensions.AssertEndElement(this XmlReader, string) Method

Tests if the current content node is an end tag whose [System.Xml.XmlReader.Name](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.Name 'System.Xml.XmlReader.Name') matches the given [name](XmlReaderExtensions.AssertEndElement(thisXmlReader,string).md#Be.Stateless.Xml.Extensions.XmlReaderExtensions.AssertEndElement(thisSystem.Xml.XmlReader,string).name 'Be.Stateless.Xml.Extensions.XmlReaderExtensions.AssertEndElement(this System.Xml.XmlReader, string).name') argument; throws otherwise.

```csharp
public static void AssertEndElement(this System.Xml.XmlReader reader, string name);
```
#### Parameters

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.AssertEndElement(thisSystem.Xml.XmlReader,string).reader'></a>

`reader` [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')

An [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') object.

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.AssertEndElement(thisSystem.Xml.XmlReader,string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string to match against the [System.Xml.XmlReader.Name](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.Name 'System.Xml.XmlReader.Name') property of the element found.