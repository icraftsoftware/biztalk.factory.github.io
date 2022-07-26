#### [Be.Stateless.BizTalk.Transform.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Transform](Be.Stateless.BizTalk.Unit.Transform.md 'Be.Stateless.BizTalk.Unit.Transform')

## ITransformFixtureXmlResult Interface

```csharp
public interface ITransformFixtureXmlResult :
Be.Stateless.BizTalk.IFluentInterface
```

Derived  
&#8627; [TransformFixtureXmlResult](TransformFixtureXmlResult.md 'Be.Stateless.BizTalk.Unit.Transform.TransformFixtureXmlResult')

Implements [IFluentInterface](IFluentInterface.md 'Be.Stateless.BizTalk.IFluentInterface')

| Properties | |
| :--- | :--- |
| [NamespaceManager](ITransformFixtureXmlResult.NamespaceManager.md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.NamespaceManager') | Namespace resolver initialized with each of the namespaces and their prefixes declared in the XSLT. |
| [XmlContent](ITransformFixtureXmlResult.XmlContent.md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.XmlContent') | The whole result of the transform as an XML string. |

| Methods | |
| :--- | :--- |
| [Evaluate(string)](ITransformFixtureXmlResult.Evaluate(string).md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.Evaluate(string)') | Evaluates the specified XPath expression and returns the typed result, implicitly using the [NamespaceManager](ITransformFixtureXmlResult.NamespaceManager.md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.NamespaceManager') to resolve namespace prefixes in the XPath expression. |
| [Matches(string)](ITransformFixtureXmlResult.Matches(string).md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.Matches(string)') | Determines whether the current node matches the specified XPath expression implicitly using the [NamespaceManager](ITransformFixtureXmlResult.NamespaceManager.md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.NamespaceManager') to resolve namespace prefixes. |
| [Select(string)](ITransformFixtureXmlResult.Select(string).md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.Select(string)') | Selects a node set using the specified XPath expression implicitly using the [NamespaceManager](ITransformFixtureXmlResult.NamespaceManager.md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.NamespaceManager') to resolve namespace prefixes in the XPath expression. |
| [SelectSingleNode(string)](ITransformFixtureXmlResult.SelectSingleNode(string).md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.SelectSingleNode(string)') | Selects a single node in the [System.Xml.XPath.XPathNavigator](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.XPathNavigator 'System.Xml.XPath.XPathNavigator') object using the specified XPath query and the implicit [NamespaceManager](ITransformFixtureXmlResult.NamespaceManager.md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.NamespaceManager') to resolve namespace prefixes. |
| [StringJoin(string, char)](ITransformFixtureXmlResult.StringJoin(string,char).md 'Be.Stateless.BizTalk.Unit.Transform.ITransformFixtureXmlResult.StringJoin(string, char)') | Concatenates all the text values of the nodes selected using the specified XPath expression and uses the specified separator between each value. |
