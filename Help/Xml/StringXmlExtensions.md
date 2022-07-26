#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Extensions](Be.Stateless.Extensions.md 'Be.Stateless.Extensions')

## StringXmlExtensions Class

```csharp
public static class StringXmlExtensions
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; StringXmlExtensions

| Methods | |
| :--- | :--- |
| [IsQName(this string)](StringXmlExtensions.IsQName(thisstring).md 'Be.Stateless.Extensions.StringXmlExtensions.IsQName(this string)') | Verifies that the [qName](StringXmlExtensions.IsQName(thisstring).md#Be.Stateless.Extensions.StringXmlExtensions.IsQName(thisstring).qName 'Be.Stateless.Extensions.StringXmlExtensions.IsQName(this string).qName') string is a valid qualified name according to the W3C Extended Markup Language recommendation. |
| [ToQName(this string, IXmlNamespaceResolver)](StringXmlExtensions.ToQName(thisstring,IXmlNamespaceResolver).md 'Be.Stateless.Extensions.StringXmlExtensions.ToQName(this string, System.Xml.IXmlNamespaceResolver)') | Given a qualified name [qName](StringXmlExtensions.ToQName(thisstring,IXmlNamespaceResolver).md#Be.Stateless.Extensions.StringXmlExtensions.ToQName(thisstring,System.Xml.IXmlNamespaceResolver).qName 'Be.Stateless.Extensions.StringXmlExtensions.ToQName(this string, System.Xml.IXmlNamespaceResolver).qName'), e.g. `ns:name` where `ns` is an xmlns prefix and `name` is an node name, and a [System.Xml.IXmlNamespaceResolver](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.IXmlNamespaceResolver 'System.Xml.IXmlNamespaceResolver')[namespaceResolver](StringXmlExtensions.ToQName(thisstring,IXmlNamespaceResolver).md#Be.Stateless.Extensions.StringXmlExtensions.ToQName(thisstring,System.Xml.IXmlNamespaceResolver).namespaceResolver 'Be.Stateless.Extensions.StringXmlExtensions.ToQName(this string, System.Xml.IXmlNamespaceResolver).namespaceResolver'), parses the [qName](StringXmlExtensions.ToQName(thisstring,IXmlNamespaceResolver).md#Be.Stateless.Extensions.StringXmlExtensions.ToQName(thisstring,System.Xml.IXmlNamespaceResolver).qName 'Be.Stateless.Extensions.StringXmlExtensions.ToQName(this string, System.Xml.IXmlNamespaceResolver).qName') string to return its typed [System.Xml.XmlQualifiedName](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlQualifiedName 'System.Xml.XmlQualifiedName') equivalent. |
| [TryParseQName(this string, string, string)](StringXmlExtensions.TryParseQName(thisstring,string,string).md 'Be.Stateless.Extensions.StringXmlExtensions.TryParseQName(this string, string, string)') | Try to parse a qualified name and extracts its prefix and local parts. |
