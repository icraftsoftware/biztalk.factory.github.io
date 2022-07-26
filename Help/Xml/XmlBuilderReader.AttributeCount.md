#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.AttributeCount Property

Gets the number of attributes on the current node.

```csharp
public override int AttributeCount { get; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks
This property is relevant to [System.Xml.XmlNodeType.DocumentType](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.DocumentType 'System.Xml.XmlNodeType.DocumentType'), [System.Xml.XmlNodeType.Element](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.Element 'System.Xml.XmlNodeType.Element'), and [System.Xml.XmlNodeType.XmlDeclaration](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.XmlDeclaration 'System.Xml.XmlNodeType.XmlDeclaration') nodes only. Other node types do not have attributes.