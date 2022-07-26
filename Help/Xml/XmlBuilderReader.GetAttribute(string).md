#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.GetAttribute(string) Method

Gets the value of the attribute with the specified [System.Xml.XmlReader.Name](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader.Name 'System.Xml.XmlReader.Name').

```csharp
public override string GetAttribute(string name);
```
#### Parameters

<a name='Be.Stateless.Xml.XmlBuilderReader.GetAttribute(string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The qualified name of the attribute.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
The value of the specified attribute. If the attribute is not found or the value is `String.Empty`, `null`
is returned.

#### Exceptions

[System.ArgumentNullException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentNullException 'System.ArgumentNullException')  
[name](XmlBuilderReader.GetAttribute(string).md#Be.Stateless.Xml.XmlBuilderReader.GetAttribute(string).name 'Be.Stateless.Xml.XmlBuilderReader.GetAttribute(string).name') is `null`.

### Remarks
This method does not move the reader.