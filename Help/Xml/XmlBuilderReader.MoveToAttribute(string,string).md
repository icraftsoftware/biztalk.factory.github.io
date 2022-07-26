#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.MoveToAttribute(string, string) Method

Moves to the attribute with the specified [System.Xml.XmlReader.LocalName](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.LocalName 'System.Xml.XmlReader.LocalName') and [System.Xml.XmlReader.NamespaceURI](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.NamespaceURI 'System.Xml.XmlReader.NamespaceURI').

```csharp
public override bool MoveToAttribute(string name, string ns);
```
#### Parameters

<a name='Be.Stateless.Xml.XmlBuilderReader.MoveToAttribute(string,string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The local name of the attribute.

<a name='Be.Stateless.Xml.XmlBuilderReader.MoveToAttribute(string,string).ns'></a>

`ns` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The namespace URI of the attribute.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if the attribute is found; `false` otherwise. If `false`, the reader's position does not
            change.

### Remarks
After calling [MoveToAttribute(string)](XmlBuilderReader.MoveToAttribute(string).md 'Be.Stateless.Xml.XmlBuilderReader.MoveToAttribute(string)'), the [System.Xml.XmlReader.Name](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.Name 'System.Xml.XmlReader.Name'), [System.Xml.XmlReader.NamespaceURI](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.NamespaceURI 'System.Xml.XmlReader.NamespaceURI'), and [System.Xml.XmlReader.Prefix](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.Prefix 'System.Xml.XmlReader.Prefix') properties reflect the properties of that
attribute.