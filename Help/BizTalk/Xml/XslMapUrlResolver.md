#### [Be.Stateless.BizTalk.Xml](README.md 'README')
### [Be.Stateless.BizTalk.Xml](Be.Stateless.BizTalk.Xml.md 'Be.Stateless.BizTalk.Xml')

## XslMapUrlResolver Class

Resolves Uniform Resource Identifiers (URIs) denoting either assembly-embedded XSLT resources or BizTalk Transform type's
strong names.

```csharp
public class XslMapUrlResolver : System.Xml.XmlUrlResolver
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.Xml.XmlResolver](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlResolver 'System.Xml.XmlResolver') &#129106; [System.Xml.XmlUrlResolver](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlUrlResolver 'System.Xml.XmlUrlResolver') &#129106; XslMapUrlResolver

### Remarks
The set of Uniform Resource Identifier (URI) that is supported is as follows:
- `map://type/<BizTalk Map's strong type name>`, for instance
              `map://type/Be.Stateless.BizTalk.Xml.Xsl.IdentityTransform, Be.Stateless.BizTalk.Xml.Tests, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14`
- `map://resource/<embedded resource's full name>`, for instance
              `map://resource/Be.Stateless.BizTalk.Xml.Data.Included.xsl`
- `map://resource/<embedded resource's name>`, for instance
              `map://resource/Data.Imported.xsl`
- `a file's absolute path without scheme`, for instance
              `C:\Files\Projects\be.stateless\BizTalkFactory\src\BizTalk.Common.Tests\Xml\Data\Imported.xsl`. Notice that this is
              natively supported by the [System.Xml.XmlUrlResolver](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlUrlResolver 'System.Xml.XmlUrlResolver') from which this class derives.

| Constructors | |
| :--- | :--- |
| [XslMapUrlResolver(Type)](XslMapUrlResolver.XslMapUrlResolver(Type).md 'Be.Stateless.BizTalk.Xml.XslMapUrlResolver.XslMapUrlResolver(System.Type)') | |

| Fields | |
| :--- | :--- |
| [MAP_SCHEME](XslMapUrlResolver.MAP_SCHEME.md 'Be.Stateless.BizTalk.Xml.XslMapUrlResolver.MAP_SCHEME') | |
| [RESOURCE_HOST](XslMapUrlResolver.RESOURCE_HOST.md 'Be.Stateless.BizTalk.Xml.XslMapUrlResolver.RESOURCE_HOST') | |
| [TYPE_HOST](XslMapUrlResolver.TYPE_HOST.md 'Be.Stateless.BizTalk.Xml.XslMapUrlResolver.TYPE_HOST') | |

| Properties | |
| :--- | :--- |
| [ReferenceType](XslMapUrlResolver.ReferenceType.md 'Be.Stateless.BizTalk.Xml.XslMapUrlResolver.ReferenceType') | |

| Methods | |
| :--- | :--- |
| [GetEntity(Uri, string, Type)](XslMapUrlResolver.GetEntity(Uri,string,Type).md 'Be.Stateless.BizTalk.Xml.XslMapUrlResolver.GetEntity(System.Uri, string, System.Type)') | Maps a URI to an object that contains the actual resource. |
| [ResolveUri(Uri, string)](XslMapUrlResolver.ResolveUri(Uri,string).md 'Be.Stateless.BizTalk.Xml.XslMapUrlResolver.ResolveUri(System.Uri, string)') | Resolves the absolute URI from the base and relative URIs. |
