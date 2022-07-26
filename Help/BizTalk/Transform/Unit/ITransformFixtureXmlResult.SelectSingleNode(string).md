#### [Be.Stateless.BizTalk.Transform.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Transform](Be.Stateless.BizTalk.Unit.Transform.md 'Be.Stateless.BizTalk.Unit.Transform').[ITransformFixtureXmlResult](ITransformFixtureXmlResult.md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult')

## ITransformFixtureXmlResult.SelectSingleNode(string) Method

Selects a single node in the [System.Xml.XPath.XPathNavigator](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.XPathNavigator 'System.Xml.XPath.XPathNavigator') object using the specified XPath query and the implicit
[NamespaceManager](ITransformFixtureXmlResult.NamespaceManager.md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.NamespaceManager') to resolve namespace prefixes.

```csharp
System.Xml.XPath.XPathNavigator SelectSingleNode(string xpath);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.SelectSingleNode(string).xpath'></a>

`xpath` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

A [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') representing an XPath expression.

#### Returns
[System.Xml.XPath.XPathNavigator](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.XPathNavigator 'System.Xml.XPath.XPathNavigator')  
An [System.Xml.XPath.XPathNavigator](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.XPathNavigator 'System.Xml.XPath.XPathNavigator') object that contains the first matching node for the XPath query specified;
otherwise [null](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/null 'https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/null') if there are no query results.