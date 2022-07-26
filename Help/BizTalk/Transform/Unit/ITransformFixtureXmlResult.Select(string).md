#### [Be.Stateless.BizTalk.Transform.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Transform](Be.Stateless.BizTalk.Unit.Transform.md 'Be.Stateless.BizTalk.Unit.Transform').[ITransformFixtureXmlResult](ITransformFixtureXmlResult.md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult')

## ITransformFixtureXmlResult.Select(string) Method

Selects a node set using the specified XPath expression implicitly using the [NamespaceManager](ITransformFixtureXmlResult.NamespaceManager.md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.NamespaceManager') to
resolve namespace prefixes in the XPath expression.

```csharp
System.Xml.XPath.XPathNodeIterator Select(string xpath);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.Select(string).xpath'></a>

`xpath` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

A [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') representing an XPath expression.

#### Returns
[System.Xml.XPath.XPathNodeIterator](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.XPathNodeIterator 'System.Xml.XPath.XPathNodeIterator')  
An [System.Xml.XPath.XPathNodeIterator](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.XPathNodeIterator 'System.Xml.XPath.XPathNodeIterator') pointing to the selected node set.