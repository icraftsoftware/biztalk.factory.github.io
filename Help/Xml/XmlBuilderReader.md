#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml')

## XmlBuilderReader Class

```csharp
public class XmlBuilderReader : System.Xml.XmlReader
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') &#129106; XmlBuilderReader

| Constructors | |
| :--- | :--- |
| [XmlBuilderReader(IXmlElementBuilder)](XmlBuilderReader.XmlBuilderReader(IXmlElementBuilder).md 'Be.Stateless.Xml.XmlBuilderReader.XmlBuilderReader(Be.Stateless.Xml.Builder.IXmlElementBuilder)') | |

| Properties | |
| :--- | :--- |
| [AttributeCount](XmlBuilderReader.AttributeCount.md 'Be.Stateless.Xml.XmlBuilderReader.AttributeCount') | Gets the number of attributes on the current node. |
| [BaseURI](XmlBuilderReader.BaseURI.md 'Be.Stateless.Xml.XmlBuilderReader.BaseURI') | Gets the base URI of the current node. |
| [CanResolveEntity](XmlBuilderReader.CanResolveEntity.md 'Be.Stateless.Xml.XmlBuilderReader.CanResolveEntity') | Gets a value indicating whether this reader can parse and resolve entities. |
| [Depth](XmlBuilderReader.Depth.md 'Be.Stateless.Xml.XmlBuilderReader.Depth') | Gets the depth of the current node in the XML document. |
| [EOF](XmlBuilderReader.EOF.md 'Be.Stateless.Xml.XmlBuilderReader.EOF') | Gets a value indicating whether the reader is positioned at the end of the stream. |
| [HasAttributes](XmlBuilderReader.HasAttributes.md 'Be.Stateless.Xml.XmlBuilderReader.HasAttributes') | Gets a value indicating whether the current node has any attributes. |
| [IsEmptyElement](XmlBuilderReader.IsEmptyElement.md 'Be.Stateless.Xml.XmlBuilderReader.IsEmptyElement') | Gets a value indicating whether the current node is an empty element (for example, <MyElement/>). |
| [LocalName](XmlBuilderReader.LocalName.md 'Be.Stateless.Xml.XmlBuilderReader.LocalName') | Gets the local name of the current node. |
| [NamespaceURI](XmlBuilderReader.NamespaceURI.md 'Be.Stateless.Xml.XmlBuilderReader.NamespaceURI') | Gets the namespace URI (as defined in the W3C Namespace specification) of the node on which the reader is positioned. |
| [NameTable](XmlBuilderReader.NameTable.md 'Be.Stateless.Xml.XmlBuilderReader.NameTable') | Gets the [System.Xml.XmlNameTable](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNameTable 'System.Xml.XmlNameTable') associated with this implementation. |
| [NodeType](XmlBuilderReader.NodeType.md 'Be.Stateless.Xml.XmlBuilderReader.NodeType') | Gets the type of the current node. |
| [Prefix](XmlBuilderReader.Prefix.md 'Be.Stateless.Xml.XmlBuilderReader.Prefix') | Gets the namespace prefix associated with the current node. |
| [ReadState](XmlBuilderReader.ReadState.md 'Be.Stateless.Xml.XmlBuilderReader.ReadState') | Gets the state of the reader. |
| [Value](XmlBuilderReader.Value.md 'Be.Stateless.Xml.XmlBuilderReader.Value') | Gets the text value of the current node. |

| Methods | |
| :--- | :--- |
| [Close()](XmlBuilderReader.Close().md 'Be.Stateless.Xml.XmlBuilderReader.Close()') | Changes the [ReadState](XmlBuilderReader.ReadState.md 'Be.Stateless.Xml.XmlBuilderReader.ReadState') to [System.Xml.ReadState.Closed](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.ReadState.Closed 'System.Xml.ReadState.Closed'). |
| [GetAttribute(int)](XmlBuilderReader.GetAttribute(int).md 'Be.Stateless.Xml.XmlBuilderReader.GetAttribute(int)') | Gets the value of the attribute with the specified index. |
| [GetAttribute(string, string)](XmlBuilderReader.GetAttribute(string,string).md 'Be.Stateless.Xml.XmlBuilderReader.GetAttribute(string, string)') | Gets the value of the attribute with the specified [System.Xml.XmlReader.LocalName](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.LocalName 'System.Xml.XmlReader.LocalName') and [System.Xml.XmlReader.NamespaceURI](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.NamespaceURI 'System.Xml.XmlReader.NamespaceURI'). |
| [GetAttribute(string)](XmlBuilderReader.GetAttribute(string).md 'Be.Stateless.Xml.XmlBuilderReader.GetAttribute(string)') | Gets the value of the attribute with the specified [System.Xml.XmlReader.Name](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.Name 'System.Xml.XmlReader.Name'). |
| [LookupNamespace(string)](XmlBuilderReader.LookupNamespace(string).md 'Be.Stateless.Xml.XmlBuilderReader.LookupNamespace(string)') | Resolves a namespace prefix in the current element's scope. |
| [MoveToAttribute(string, string)](XmlBuilderReader.MoveToAttribute(string,string).md 'Be.Stateless.Xml.XmlBuilderReader.MoveToAttribute(string, string)') | Moves to the attribute with the specified [System.Xml.XmlReader.LocalName](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.LocalName 'System.Xml.XmlReader.LocalName') and [System.Xml.XmlReader.NamespaceURI](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.NamespaceURI 'System.Xml.XmlReader.NamespaceURI'). |
| [MoveToAttribute(string)](XmlBuilderReader.MoveToAttribute(string).md 'Be.Stateless.Xml.XmlBuilderReader.MoveToAttribute(string)') | Moves to the attribute with the specified [System.Xml.XmlReader.Name](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.Name 'System.Xml.XmlReader.Name'). |
| [MoveToElement()](XmlBuilderReader.MoveToElement().md 'Be.Stateless.Xml.XmlBuilderReader.MoveToElement()') | When overridden in a derived class, moves to the element that contains the current attribute node. |
| [MoveToFirstAttribute()](XmlBuilderReader.MoveToFirstAttribute().md 'Be.Stateless.Xml.XmlBuilderReader.MoveToFirstAttribute()') | Moves to the first attribute. |
| [MoveToNextAttribute()](XmlBuilderReader.MoveToNextAttribute().md 'Be.Stateless.Xml.XmlBuilderReader.MoveToNextAttribute()') | Moves to the next attribute. |
| [Read()](XmlBuilderReader.Read().md 'Be.Stateless.Xml.XmlBuilderReader.Read()') | Reads the next node from the stream. |
| [ReadAttributeValue()](XmlBuilderReader.ReadAttributeValue().md 'Be.Stateless.Xml.XmlBuilderReader.ReadAttributeValue()') | Parses the attribute value into one or more [System.Xml.XmlNodeType.Text](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.Text 'System.Xml.XmlNodeType.Text'), [System.Xml.XmlNodeType.EntityReference](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.EntityReference 'System.Xml.XmlNodeType.EntityReference'), or [System.Xml.XmlNodeType.EndEntity](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.EndEntity 'System.Xml.XmlNodeType.EndEntity') nodes. |
| [ResolveEntity()](XmlBuilderReader.ResolveEntity().md 'Be.Stateless.Xml.XmlBuilderReader.ResolveEntity()') | Resolves the entity reference for [System.Xml.XmlNodeType.EntityReference](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.EntityReference 'System.Xml.XmlNodeType.EntityReference') nodes. |
