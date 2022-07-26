#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.MoveToFirstAttribute() Method

Moves to the first attribute.

```csharp
public override bool MoveToFirstAttribute();
```

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if an attribute exists; `false` otherwise.

### Remarks
If [MoveToFirstAttribute()](XmlBuilderReader.MoveToFirstAttribute().md 'Be.Stateless.Xml.XmlBuilderReader.MoveToFirstAttribute()') returns `true`, the reader moves to the first attribute; otherwise, the
position of the reader does not change.