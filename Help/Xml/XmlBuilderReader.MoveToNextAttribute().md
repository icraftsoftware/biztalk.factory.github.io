#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.MoveToNextAttribute() Method

Moves to the next attribute.

```csharp
public override bool MoveToNextAttribute();
```

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if there is a next attribute; `false` if there are no more attributes.

### Remarks
If the current node is an element node, this method is equivalent to [MoveToFirstAttribute()](XmlBuilderReader.MoveToFirstAttribute().md 'Be.Stateless.Xml.XmlBuilderReader.MoveToFirstAttribute()'). If [MoveToNextAttribute()](XmlBuilderReader.MoveToNextAttribute().md 'Be.Stateless.Xml.XmlBuilderReader.MoveToNextAttribute()') returns `true`, the reader moves to the next attribute; otherwise, the position of
the reader does not change.