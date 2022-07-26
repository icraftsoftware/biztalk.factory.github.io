#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.IsEmptyElement Property

Gets a value indicating whether the current node is an empty element (for example, <MyElement/>).

```csharp
public override bool IsEmptyElement { get; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

This property enables you to determine the difference between the following:
- <item num="123"/>, for which [IsEmptyElement](XmlBuilderReader.IsEmptyElement.md 'Be.Stateless.Xml.XmlBuilderReader.IsEmptyElement') is `true`;
- <item num="123"></item>, for which [IsEmptyElement](XmlBuilderReader.IsEmptyElement.md 'Be.Stateless.Xml.XmlBuilderReader.IsEmptyElement') is `false` although element content
              is empty.
A corresponding [System.Xml.XmlNodeType.EndElement](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNodeType.EndElement 'System.Xml.XmlNodeType.EndElement') node is not generated for empty elements.

If default content has been added to an element due to schema validation, [IsEmptyElement](XmlBuilderReader.IsEmptyElement.md 'Be.Stateless.Xml.XmlBuilderReader.IsEmptyElement') still returns
`true`. It has no bearing on whether or not the element has a default value. In other words, [IsEmptyElement](XmlBuilderReader.IsEmptyElement.md 'Be.Stateless.Xml.XmlBuilderReader.IsEmptyElement') simply reports whether or not the element in the source document had an end element tag.