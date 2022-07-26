#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Extensions](Be.Stateless.Extensions.md 'Be.Stateless.Extensions').[StringXmlExtensions](StringXmlExtensions.md 'Be.Stateless.Extensions.StringXmlExtensions')

## StringXmlExtensions.ToQName(this string, IXmlNamespaceResolver) Method

Given a qualified name [qName](StringXmlExtensions.ToQName(thisstring,IXmlNamespaceResolver).md#Be.Stateless.Extensions.StringXmlExtensions.ToQName(thisstring,System.Xml.IXmlNamespaceResolver).qName 'Be.Stateless.Extensions.StringXmlExtensions.ToQName(this string, System.Xml.IXmlNamespaceResolver).qName'), e.g. `ns:name` where `ns` is an xmlns prefix and
`name` is an node name, and a [System.Xml.IXmlNamespaceResolver](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.IXmlNamespaceResolver 'System.Xml.IXmlNamespaceResolver')[namespaceResolver](StringXmlExtensions.ToQName(thisstring,IXmlNamespaceResolver).md#Be.Stateless.Extensions.StringXmlExtensions.ToQName(thisstring,System.Xml.IXmlNamespaceResolver).namespaceResolver 'Be.Stateless.Extensions.StringXmlExtensions.ToQName(this string, System.Xml.IXmlNamespaceResolver).namespaceResolver'), parses
the [qName](StringXmlExtensions.ToQName(thisstring,IXmlNamespaceResolver).md#Be.Stateless.Extensions.StringXmlExtensions.ToQName(thisstring,System.Xml.IXmlNamespaceResolver).qName 'Be.Stateless.Extensions.StringXmlExtensions.ToQName(this string, System.Xml.IXmlNamespaceResolver).qName') string to return its typed [System.Xml.XmlQualifiedName](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlQualifiedName 'System.Xml.XmlQualifiedName') equivalent.

```csharp
public static System.Xml.XmlQualifiedName ToQName(this string qName, System.Xml.IXmlNamespaceResolver namespaceResolver);
```
#### Parameters

<a name='Be.Stateless.Extensions.StringXmlExtensions.ToQName(thisstring,System.Xml.IXmlNamespaceResolver).qName'></a>

`qName` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The qName string to parse.

<a name='Be.Stateless.Extensions.StringXmlExtensions.ToQName(thisstring,System.Xml.IXmlNamespaceResolver).namespaceResolver'></a>

`namespaceResolver` [System.Xml.IXmlNamespaceResolver](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.IXmlNamespaceResolver 'System.Xml.IXmlNamespaceResolver')

The [System.Xml.IXmlNamespaceResolver](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.IXmlNamespaceResolver 'System.Xml.IXmlNamespaceResolver') to use to resolve the xmlns prefix of the [qName](StringXmlExtensions.ToQName(thisstring,IXmlNamespaceResolver).md#Be.Stateless.Extensions.StringXmlExtensions.ToQName(thisstring,System.Xml.IXmlNamespaceResolver).qName 'Be.Stateless.Extensions.StringXmlExtensions.ToQName(this string, System.Xml.IXmlNamespaceResolver).qName').

#### Returns
[System.Xml.XmlQualifiedName](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlQualifiedName 'System.Xml.XmlQualifiedName')  
The typed [System.Xml.XmlQualifiedName](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlQualifiedName 'System.Xml.XmlQualifiedName') equivalent of the [qName](StringXmlExtensions.ToQName(thisstring,IXmlNamespaceResolver).md#Be.Stateless.Extensions.StringXmlExtensions.ToQName(thisstring,System.Xml.IXmlNamespaceResolver).qName 'Be.Stateless.Extensions.StringXmlExtensions.ToQName(this string, System.Xml.IXmlNamespaceResolver).qName').