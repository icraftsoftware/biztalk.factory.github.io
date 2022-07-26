#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml.XPath](Be.Stateless.Xml.XPath.md 'Be.Stateless.Xml.XPath')

## NamespaceAffinitiveXPathNavigator Class

[XPathNavigatorDecorator](XPathNavigatorDecorator.md 'Be.Stateless.Xml.XPath.XPathNavigatorDecorator') that propagates the [NamespaceManager](NamespaceAffinitiveXPathNavigator.NamespaceManager.md 'Be.Stateless.Xml.XPath.NamespaceAffinitiveXPathNavigator.NamespaceManager') further down the resulting [System.Xml.XPath.XPathNavigator](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.XPathNavigator 'System.Xml.XPath.XPathNavigator')
            and [System.Xml.XPath.XPathNodeIterator](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.XPathNodeIterator 'System.Xml.XPath.XPathNodeIterator') and consequently allows subsequent XPath queries to be implicitly scoped by the XML
            namespaces that are propagated by the [NamespaceManager](NamespaceAffinitiveXPathNavigator.NamespaceManager.md 'Be.Stateless.Xml.XPath.NamespaceAffinitiveXPathNavigator.NamespaceManager').

```csharp
public class NamespaceAffinitiveXPathNavigator : Be.Stateless.Xml.XPath.XPathNavigatorDecorator
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.Xml.XPath.XPathItem](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.XPathItem 'System.Xml.XPath.XPathItem') &#129106; [System.Xml.XPath.XPathNavigator](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.XPathNavigator 'System.Xml.XPath.XPathNavigator') &#129106; [XPathNavigatorDecorator](XPathNavigatorDecorator.md 'Be.Stateless.Xml.XPath.XPathNavigatorDecorator') &#129106; NamespaceAffinitiveXPathNavigator

| Constructors | |
| :--- | :--- |
| [NamespaceAffinitiveXPathNavigator(XPathNavigator, XmlNamespaceManager)](NamespaceAffinitiveXPathNavigator.NamespaceAffinitiveXPathNavigator(XPathNavigator,XmlNamespaceManager).md 'Be.Stateless.Xml.XPath.NamespaceAffinitiveXPathNavigator.NamespaceAffinitiveXPathNavigator(System.Xml.XPath.XPathNavigator, System.Xml.XmlNamespaceManager)') | |

| Properties | |
| :--- | :--- |
| [NamespaceManager](NamespaceAffinitiveXPathNavigator.NamespaceManager.md 'Be.Stateless.Xml.XPath.NamespaceAffinitiveXPathNavigator.NamespaceManager') | |

| Methods | |
| :--- | :--- |
| [CreateXPathNavigatorDecorator(XPathNavigator)](NamespaceAffinitiveXPathNavigator.CreateXPathNavigatorDecorator(XPathNavigator).md 'Be.Stateless.Xml.XPath.NamespaceAffinitiveXPathNavigator.CreateXPathNavigatorDecorator(System.Xml.XPath.XPathNavigator)') | |
| [Evaluate(string)](NamespaceAffinitiveXPathNavigator.Evaluate(string).md 'Be.Stateless.Xml.XPath.NamespaceAffinitiveXPathNavigator.Evaluate(string)') | |
| [Matches(string)](NamespaceAffinitiveXPathNavigator.Matches(string).md 'Be.Stateless.Xml.XPath.NamespaceAffinitiveXPathNavigator.Matches(string)') | |
| [Select(string)](NamespaceAffinitiveXPathNavigator.Select(string).md 'Be.Stateless.Xml.XPath.NamespaceAffinitiveXPathNavigator.Select(string)') | |
| [SelectSingleNode(string)](NamespaceAffinitiveXPathNavigator.SelectSingleNode(string).md 'Be.Stateless.Xml.XPath.NamespaceAffinitiveXPathNavigator.SelectSingleNode(string)') | |
