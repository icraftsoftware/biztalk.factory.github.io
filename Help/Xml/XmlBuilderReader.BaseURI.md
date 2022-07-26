#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.BaseURI Property

Gets the base URI of the current node.

```csharp
public override string BaseURI { get; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
A networked XML document is comprised of chunks of data aggregated using various W3C standard inclusion mechanisms
and therefore contains nodes that come from different places. DTD entities are an example of this, but this is not
limited to DTDs. The [BaseURI](XmlBuilderReader.BaseURI.md 'Be.Stateless.Xml.XmlBuilderReader.BaseURI') tells you where these nodes came from. If there is no base URI for the
nodes being returned (for example, they were parsed from an in-memory string), `String.Empty` is returned.