#### [Be.Stateless.BizTalk.Xml](README.md 'README')
### [Be.Stateless.BizTalk.Xml](Be.Stateless.BizTalk.Xml.md 'Be.Stateless.BizTalk.Xml').[XslMapUrlResolver](XslMapUrlResolver.md 'Be.Stateless.BizTalk.Xml.XslMapUrlResolver')

## XslMapUrlResolver.GetEntity(Uri, string, Type) Method

Maps a URI to an object that contains the actual resource.

```csharp
public override object GetEntity(System.Uri absoluteUri, string role, System.Type ofObjectToReturn);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Xml.XslMapUrlResolver.GetEntity(System.Uri,string,System.Type).absoluteUri'></a>

`absoluteUri` [System.Uri](https://docs.microsoft.com/en-us/dotnet/api/System.Uri 'System.Uri')

The URI returned from [ResolveUri(Uri, string)](XslMapUrlResolver.ResolveUri(Uri,string).md 'Be.Stateless.BizTalk.Xml.XslMapUrlResolver.ResolveUri(System.Uri, string)').

<a name='Be.Stateless.BizTalk.Xml.XslMapUrlResolver.GetEntity(System.Uri,string,System.Type).role'></a>

`role` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

Currently not used.

<a name='Be.Stateless.BizTalk.Xml.XslMapUrlResolver.GetEntity(System.Uri,string,System.Type).ofObjectToReturn'></a>

`ofObjectToReturn` [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')

The type of object to return.

#### Returns
[System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')  
One of [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream'), [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader'), or [System.Xml.XPath.IXPathNavigable](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.IXPathNavigable 'System.Xml.XPath.IXPathNavigable').