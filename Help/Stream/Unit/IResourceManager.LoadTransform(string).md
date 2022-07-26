#### [Be.Stateless.Stream.Unit](README.md 'README')
### [Be.Stateless.Unit.Resources](Be.Stateless.Unit.Resources.md 'Be.Stateless.Unit.Resources').[IResourceManager](IResourceManager.md 'Be.Stateless.Unit.Resources.IResourceManager')

## IResourceManager.LoadTransform(string) Method

Loads and deserializes an [System.Xml.Xsl.XslCompiledTransform](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XslCompiledTransform 'System.Xml.Xsl.XslCompiledTransform') embedded in the calling assembly.

```csharp
System.Xml.Xsl.XslCompiledTransform LoadTransform(string name);
```
#### Parameters

<a name='Be.Stateless.Unit.Resources.IResourceManager.LoadTransform(string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name of the [System.Xml.Xsl.XslCompiledTransform](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XslCompiledTransform 'System.Xml.Xsl.XslCompiledTransform') resource.

#### Returns
[System.Xml.Xsl.XslCompiledTransform](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XslCompiledTransform 'System.Xml.Xsl.XslCompiledTransform')  
The deserialized [System.Xml.Xsl.XslCompiledTransform](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XslCompiledTransform 'System.Xml.Xsl.XslCompiledTransform').