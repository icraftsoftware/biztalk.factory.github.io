#### [Be.Stateless.BizTalk.Transform.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Transform](Be.Stateless.BizTalk.Unit.Transform.md 'Be.Stateless.BizTalk.Unit.Transform').[MapCustomXsltPathResolver](MapCustomXsltPathResolver.md 'Be.Stateless.BizTalk.Unit.Transform.MapCustomXsltPathResolver')

## MapCustomXsltPathResolver.TryResolveEmbeddedXsltResourceSourceFilePath(this Type, string, string) Method

Resolve the path to an XSLT embedded in a custom BizTalk map, given this map's type to initiate probing.

```csharp
public static bool TryResolveEmbeddedXsltResourceSourceFilePath(this System.Type type, string resource, out string path);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Transform.MapCustomXsltPathResolver.TryResolveEmbeddedXsltResourceSourceFilePath(thisSystem.Type,string,string).type'></a>

`type` [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')

The BizTalk map type to be used to initiate the probing.

<a name='Be.Stateless.BizTalk.Unit.Transform.MapCustomXsltPathResolver.TryResolveEmbeddedXsltResourceSourceFilePath(thisSystem.Type,string,string).resource'></a>

`resource` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name of the resource to probe for its source XSLT file.

<a name='Be.Stateless.BizTalk.Unit.Transform.MapCustomXsltPathResolver.TryResolveEmbeddedXsltResourceSourceFilePath(thisSystem.Type,string,string).path'></a>

`path` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The resolved path to the embedded XSLT.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if the path to the source of the embedded XSLT could be resolved; `false` otherwise.

### See Also
- [Be.Stateless.BizTalk.Xml.XslMapUrlResolver](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Xml.XslMapUrlResolver 'Be.Stateless.BizTalk.Xml.XslMapUrlResolver')