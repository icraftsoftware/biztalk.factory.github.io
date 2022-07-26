#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.MoveToElement() Method

When overridden in a derived class, moves to the element that contains the current attribute node.

```csharp
public override bool MoveToElement();
```

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if the reader is positioned on an attribute (the reader moves to the element that owns the attribute);
            `false` if the reader is not positioned on an attribute (the position of the reader does not change).

### Remarks
Use this method to return to an element after navigating through its attributes. This method moves the reader to one
of the following node types: [System.Xml.XmlNodeType.DocumentType](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.DocumentType 'System.Xml.XmlNodeType.DocumentType'), [System.Xml.XmlNodeType.Element](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.Element 'System.Xml.XmlNodeType.Element'), or [System.Xml.XmlNodeType.XmlDeclaration](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.XmlDeclaration 'System.Xml.XmlNodeType.XmlDeclaration').