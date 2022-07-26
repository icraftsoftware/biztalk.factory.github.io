#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml.Extensions](Be.Stateless.Xml.Extensions.md 'Be.Stateless.Xml.Extensions').[XmlReaderExtensions](XmlReaderExtensions.md 'Be.Stateless.Xml.Extensions.XmlReaderExtensions')

## XmlReaderExtensions.AssertStartElement(this XmlReader, string) Method

Calls [System.Xml.XmlReader.MoveToContent](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.MoveToContent 'System.Xml.XmlReader.MoveToContent') and tests if the current content node is a start tag or empty element tag
whose [System.Xml.XmlReader.Name](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.Name 'System.Xml.XmlReader.Name') matches the given [name](XmlReaderExtensions.AssertStartElement(thisXmlReader,string).md#Be.Stateless.Xml.Extensions.XmlReaderExtensions.AssertStartElement(thisSystem.Xml.XmlReader,string).name 'Be.Stateless.Xml.Extensions.XmlReaderExtensions.AssertStartElement(this System.Xml.XmlReader, string).name') argument; throws otherwise.

```csharp
public static void AssertStartElement(this System.Xml.XmlReader reader, string name);
```
#### Parameters

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.AssertStartElement(thisSystem.Xml.XmlReader,string).reader'></a>

`reader` [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')

An [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') object.

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.AssertStartElement(thisSystem.Xml.XmlReader,string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string to match against the [System.Xml.XmlReader.Name](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.Name 'System.Xml.XmlReader.Name') property of the element found.