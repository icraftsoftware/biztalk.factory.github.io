#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml.Extensions](Be.Stateless.Xml.Extensions.md 'Be.Stateless.Xml.Extensions').[XmlReaderExtensions](XmlReaderExtensions.md 'Be.Stateless.Xml.Extensions.XmlReaderExtensions')

## XmlReaderExtensions.AssertStartElement(this XmlReader, string, string) Method

Calls [System.Xml.XmlReader.MoveToContent](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.MoveToContent 'System.Xml.XmlReader.MoveToContent') and tests if the current content node is a start tag or empty element tag
whose [System.Xml.XmlReader.LocalName](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.LocalName 'System.Xml.XmlReader.LocalName') and [System.Xml.XmlReader.NamespaceURI](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.NamespaceURI 'System.Xml.XmlReader.NamespaceURI') properties match the given [name](XmlReaderExtensions.AssertStartElement(thisXmlReader,string,string).md#Be.Stateless.Xml.Extensions.XmlReaderExtensions.AssertStartElement(thisSystem.Xml.XmlReader,string,string).name 'Be.Stateless.Xml.Extensions.XmlReaderExtensions.AssertStartElement(this System.Xml.XmlReader, string, string).name') and [ns](XmlReaderExtensions.AssertStartElement(thisXmlReader,string,string).md#Be.Stateless.Xml.Extensions.XmlReaderExtensions.AssertStartElement(thisSystem.Xml.XmlReader,string,string).ns 'Be.Stateless.Xml.Extensions.XmlReaderExtensions.AssertStartElement(this System.Xml.XmlReader, string, string).ns') arguments; throws otherwise.

```csharp
public static void AssertStartElement(this System.Xml.XmlReader reader, string name, string ns);
```
#### Parameters

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.AssertStartElement(thisSystem.Xml.XmlReader,string,string).reader'></a>

`reader` [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')

An [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') object.

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.AssertStartElement(thisSystem.Xml.XmlReader,string,string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string to match against the [System.Xml.XmlReader.LocalName](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.LocalName 'System.Xml.XmlReader.LocalName') property of the element found.

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.AssertStartElement(thisSystem.Xml.XmlReader,string,string).ns'></a>

`ns` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string to match against the [System.Xml.XmlReader.NamespaceURI](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.NamespaceURI 'System.Xml.XmlReader.NamespaceURI') property of the element found.