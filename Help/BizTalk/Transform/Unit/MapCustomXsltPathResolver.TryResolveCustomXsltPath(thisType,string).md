#### [Be.Stateless.BizTalk.Transform.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Transform](Be.Stateless.BizTalk.Unit.Transform.md 'Be.Stateless.BizTalk.Unit.Transform').[MapCustomXsltPathResolver](MapCustomXsltPathResolver.md 'Be.Stateless.BizTalk.Unit.Transform.MapCustomXsltPathResolver')

## MapCustomXsltPathResolver.TryResolveCustomXsltPath(this Type, string) Method

Resolve the path to a BizTalk map's custom XSLT.

```csharp
public static bool TryResolveCustomXsltPath(this System.Type type, out string path);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Transform.MapCustomXsltPathResolver.TryResolveCustomXsltPath(thisSystem.Type,string).type'></a>

`type` [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')

The BizTalk map for which the path to the custom XSLT should be resolved.

<a name='Be.Stateless.BizTalk.Unit.Transform.MapCustomXsltPathResolver.TryResolveCustomXsltPath(thisSystem.Type,string).path'></a>

`path` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The resolved path to the custom XSLT of the BizTalk map passed.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if the path to the source of the custom XSLT could be resolved; `false` otherwise.

### Remarks

For its path to be resolved, the custom XSLT source file must reside, by convention, next to its `.btm` file and
have the same name except for the extension that must either be `.xsl` or `.xslt`.

Technically, [MapCustomXsltPathResolver](MapCustomXsltPathResolver.md 'Be.Stateless.BizTalk.Unit.Transform.MapCustomXsltPathResolver') will first try lo locate the `.pdb` file of the transform
type's assembly. If successful, it will then try to retrieve from the debug information the path of the generated
`.btm.cs` source file of the [Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase')-derived class. If successful, it will finally try to
locate an `.xsl` or `.xslt` file next to the `.btm.cs` (i.e. with the same name except for the
`.btm.cs` extension).