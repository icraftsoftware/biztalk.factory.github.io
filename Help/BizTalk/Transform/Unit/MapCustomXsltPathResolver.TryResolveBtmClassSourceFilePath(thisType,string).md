#### [Be.Stateless.BizTalk.Transform.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Transform](Be.Stateless.BizTalk.Unit.Transform.md 'Be.Stateless.BizTalk.Unit.Transform').[MapCustomXsltPathResolver](MapCustomXsltPathResolver.md 'Be.Stateless.BizTalk.Unit.Transform.MapCustomXsltPathResolver')

## MapCustomXsltPathResolver.TryResolveBtmClassSourceFilePath(this Type, string) Method

Resolve the path to a BizTalk map class source file, i.e. the .btm.cs compiler generated source file.

```csharp
public static bool TryResolveBtmClassSourceFilePath(this System.Type type, out string path);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Transform.MapCustomXsltPathResolver.TryResolveBtmClassSourceFilePath(thisSystem.Type,string).type'></a>

`type` [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')

The BizTalk map type for which the path to the source file should be resolved.

<a name='Be.Stateless.BizTalk.Unit.Transform.MapCustomXsltPathResolver.TryResolveBtmClassSourceFilePath(thisSystem.Type,string).path'></a>

`path` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The resolved path to the source BizTalk map type.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if the path to the source file of the BizTalk map type could be resolved; `false` otherwise.