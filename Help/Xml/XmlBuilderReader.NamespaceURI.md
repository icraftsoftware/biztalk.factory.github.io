#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.NamespaceURI Property

Gets the namespace URI (as defined in the W3C Namespace specification) of the node on which the reader is positioned.

```csharp
public override string NamespaceURI { get; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
This property is relevant to [System.Xml.XmlNodeType.Attribute](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.Attribute 'System.Xml.XmlNodeType.Attribute') and [System.Xml.XmlNodeType.Element](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.Element 'System.Xml.XmlNodeType.Element') nodes only.