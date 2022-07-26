#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml.Extensions](Be.Stateless.Xml.Extensions.md 'Be.Stateless.Xml.Extensions').[XmlReaderExtensions](XmlReaderExtensions.md 'Be.Stateless.Xml.Extensions.XmlReaderExtensions')

## XmlReaderExtensions.ReadEndElement(this XmlReader, string) Method

Checks that the current content node is an element with the given [name](XmlReaderExtensions.ReadEndElement(thisXmlReader,string).md#Be.Stateless.Xml.Extensions.XmlReaderExtensions.ReadEndElement(thisSystem.Xml.XmlReader,string).name 'Be.Stateless.Xml.Extensions.XmlReaderExtensions.ReadEndElement(this System.Xml.XmlReader, string).name') name="name"/> and advances
the reader to the next node.

```csharp
public static void ReadEndElement(this System.Xml.XmlReader reader, string name);
```
#### Parameters

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.ReadEndElement(thisSystem.Xml.XmlReader,string).reader'></a>

`reader` [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')

An [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') object.

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.ReadEndElement(thisSystem.Xml.XmlReader,string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The qualified name of the element.