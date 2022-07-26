#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.Read() Method

Reads the next node from the stream.

```csharp
public override bool Read();
```

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if the next node was read successfully; `false` if there are no more nodes to read.

#### Exceptions

[System.Xml.XmlException](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlException 'System.Xml.XmlException')  
An error occurred while parsing the XML.

### Remarks
When an [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') is first created and initialized, there is no information available. You must call
[Read()](XmlBuilderReader.Read().md 'Be.Stateless.Xml.XmlBuilderReader.Read()') to read the first node.