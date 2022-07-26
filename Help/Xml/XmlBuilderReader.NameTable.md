#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.NameTable Property

Gets the [System.Xml.XmlNameTable](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNameTable 'System.Xml.XmlNameTable') associated with this implementation.

```csharp
public override System.Xml.XmlNameTable NameTable { get; }
```

#### Property Value
[System.Xml.XmlNameTable](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNameTable 'System.Xml.XmlNameTable')

### Remarks
All node and attribute names returned from XmlReader are atomized using the [System.Xml.XmlNameTable](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNameTable 'System.Xml.XmlNameTable'). When the same
name is returned multiple times (for example, `Customer`), then the same [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') object will be
returned for that name. This makes it possible for you to write efficient code that does object comparisons on these
strings instead of expensive string comparisons