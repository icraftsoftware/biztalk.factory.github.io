#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.ReadAttributeValue() Method

Parses the attribute value into one or more [System.Xml.XmlNodeType.Text](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.Text 'System.Xml.XmlNodeType.Text'), [System.Xml.XmlNodeType.EntityReference](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.EntityReference 'System.Xml.XmlNodeType.EntityReference'), or [System.Xml.XmlNodeType.EndEntity](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.EndEntity 'System.Xml.XmlNodeType.EndEntity') nodes.

```csharp
public override bool ReadAttributeValue();
```

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if there are nodes to return. `false` if the reader is not positioned on an attribute node when the
            initial call is made or if all the attribute values have been read. An empty attribute, such as,
            `misc=""`, returns `true`
            with a single node with a value of `String.Empty`.

### Remarks
Use this method after calling [MoveToAttribute(string)](XmlBuilderReader.MoveToAttribute(string).md 'Be.Stateless.Xml.XmlBuilderReader.MoveToAttribute(string)') to read through the text or entity reference
nodes that make up the attribute value. The [System.Xml.XmlReader.Depth](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.Depth 'System.Xml.XmlReader.Depth') of the attribute value nodes is one plus
the depth of the attribute node; it increments and decrements by one when you step into and out of general entity
references.