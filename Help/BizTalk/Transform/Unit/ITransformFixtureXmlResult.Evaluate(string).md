#### [Be.Stateless.BizTalk.Transform.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Transform](Be.Stateless.BizTalk.Unit.Transform.md 'Be.Stateless.BizTalk.Unit.Transform').[ITransformFixtureXmlResult](ITransformFixtureXmlResult.md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult')

## ITransformFixtureXmlResult.Evaluate(string) Method

Evaluates the specified XPath expression and returns the typed result, implicitly using the [NamespaceManager](ITransformFixtureXmlResult.NamespaceManager.md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.NamespaceManager') to resolve namespace prefixes in the XPath expression.

```csharp
object Evaluate(string xpath);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.Evaluate(string).xpath'></a>

`xpath` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

A [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') representing an XPath expression that can be evaluated.

#### Returns
[System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')  
The result of the expression, either a Boolean, a number, a string, or a node set. This maps to [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean'),
[System.Double](https://docs.microsoft.com/en-us/dotnet/api/System.Double 'System.Double'), [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String'), or [System.Xml.XPath.XPathNodeIterator](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.XPathNodeIterator 'System.Xml.XPath.XPathNodeIterator') objects
respectively.