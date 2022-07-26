#### [Be.Stateless.BizTalk.Xml](README.md 'README')
### [Be.Stateless.BizTalk.Xml](Be.Stateless.BizTalk.Xml.md 'Be.Stateless.BizTalk.Xml').[XslMapUrlResolver](XslMapUrlResolver.md 'Be.Stateless.BizTalk.Xml.XslMapUrlResolver')

## XslMapUrlResolver.ResolveUri(Uri, string) Method

Resolves the absolute URI from the base and relative URIs.

```csharp
public override System.Uri ResolveUri(System.Uri baseUri, string relativeUri);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Xml.XslMapUrlResolver.ResolveUri(System.Uri,string).baseUri'></a>

`baseUri` [System.Uri](https://docs.microsoft.com/en-us/dotnet/api/System.Uri 'System.Uri')

The base URI used to resolve the relative URI.

<a name='Be.Stateless.BizTalk.Xml.XslMapUrlResolver.ResolveUri(System.Uri,string).relativeUri'></a>

`relativeUri` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The URI to resolve. The URI can be absolute or relative. If absolute, this value effectively replaces the baseUri
value. If relative, it combines with the baseUri to make an absolute URI.

#### Returns
[System.Uri](https://docs.microsoft.com/en-us/dotnet/api/System.Uri 'System.Uri')  
The absolute URI or null if the relative URI cannot be resolved.