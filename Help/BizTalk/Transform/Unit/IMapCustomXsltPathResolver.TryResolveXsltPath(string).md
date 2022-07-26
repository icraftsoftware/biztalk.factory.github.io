#### [Be.Stateless.BizTalk.Transform.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Transform](Be.Stateless.BizTalk.Unit.Transform.md 'Be.Stateless.BizTalk.Unit.Transform').[IMapCustomXsltPathResolver](IMapCustomXsltPathResolver.md 'Be.Stateless.BizTalk.Unit.Transform.IMapCustomXsltPathResolver')

## IMapCustomXsltPathResolver.TryResolveXsltPath(string) Method

Resolve the path to a BizTalk map's custom XSLT.

```csharp
bool TryResolveXsltPath(out string path);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Transform.IMapCustomXsltPathResolver.TryResolveXsltPath(string).path'></a>

`path` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The resolved path to the custom XSLT of the BizTalk map passed to the constructor.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if the path to the source of the custom XSLT could be resolved; `false` otherwise.