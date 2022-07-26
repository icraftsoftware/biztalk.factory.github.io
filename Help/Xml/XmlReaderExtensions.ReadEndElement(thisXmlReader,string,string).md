#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml.Extensions](Be.Stateless.Xml.Extensions.md 'Be.Stateless.Xml.Extensions').[XmlReaderExtensions](XmlReaderExtensions.md 'Be.Stateless.Xml.Extensions.XmlReaderExtensions')

## XmlReaderExtensions.ReadEndElement(this XmlReader, string, string) Method

Checks that the current content node is an element with the given [System.Xml.XmlReader.LocalName](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.LocalName 'System.Xml.XmlReader.LocalName') and [System.Xml.XmlReader.NamespaceURI](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.NamespaceURI 'System.Xml.XmlReader.NamespaceURI') and advances the reader to the next node.

```csharp
public static void ReadEndElement(this System.Xml.XmlReader reader, string name, string ns);
```
#### Parameters

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.ReadEndElement(thisSystem.Xml.XmlReader,string,string).reader'></a>

`reader` [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')

An [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') object.

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.ReadEndElement(thisSystem.Xml.XmlReader,string,string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The local name of the element.

<a name='Be.Stateless.Xml.Extensions.XmlReaderExtensions.ReadEndElement(thisSystem.Xml.XmlReader,string,string).ns'></a>

`ns` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The namespace URI of the element.