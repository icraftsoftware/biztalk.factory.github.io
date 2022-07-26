#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.ResolveEntity() Method

Resolves the entity reference for [System.Xml.XmlNodeType.EntityReference](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.EntityReference 'System.Xml.XmlNodeType.EntityReference') nodes.

```csharp
public override void ResolveEntity();
```

#### Exceptions

[System.InvalidOperationException](https://docs.microsoft.com/en-us/dotnet/api/System.InvalidOperationException 'System.InvalidOperationException')  
The reader is not positioned on an [System.Xml.XmlNodeType.EntityReference](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.EntityReference 'System.Xml.XmlNodeType.EntityReference') node or this implementation of the
reader cannot resolve entities ([System.Xml.XmlReader.CanResolveEntity](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.CanResolveEntity 'System.Xml.XmlReader.CanResolveEntity') returns `false`).

### Remarks
If the reader is positioned on an [System.Xml.XmlNodeType.EntityReference](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.EntityReference 'System.Xml.XmlNodeType.EntityReference') node, if [Read()](XmlBuilderReader.Read().md 'Be.Stateless.Xml.XmlBuilderReader.Read()') is called
after calling this method, the entity replacement text is parsed. When the entity replacement text is finished, an
[System.Xml.XmlNodeType.EndEntity](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.EndEntity 'System.Xml.XmlNodeType.EndEntity') node is returned to close the entity reference scope.