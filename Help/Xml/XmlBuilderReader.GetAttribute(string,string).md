#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.GetAttribute(string, string) Method

Gets the value of the attribute with the specified [System.Xml.XmlReader.LocalName](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.LocalName 'System.Xml.XmlReader.LocalName') and [System.Xml.XmlReader.NamespaceURI](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.NamespaceURI 'System.Xml.XmlReader.NamespaceURI').

```csharp
public override string GetAttribute(string name, string namespaceUri);
```
#### Parameters

<a name='Be.Stateless.Xml.XmlBuilderReader.GetAttribute(string,string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The local name of the attribute.

<a name='Be.Stateless.Xml.XmlBuilderReader.GetAttribute(string,string).namespaceUri'></a>

`namespaceUri` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The namespace URI of the attribute.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
The value of the specified attribute. If the attribute is not found or the value is `String.Empty`, `null`
is returned.

#### Exceptions

[System.ArgumentNullException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentNullException 'System.ArgumentNullException')  
[name](XmlBuilderReader.GetAttribute(string,string).md#Be.Stateless.Xml.XmlBuilderReader.GetAttribute(string,string).name 'Be.Stateless.Xml.XmlBuilderReader.GetAttribute(string, string).name') is `null`.

### Remarks
This method does not move the reader.