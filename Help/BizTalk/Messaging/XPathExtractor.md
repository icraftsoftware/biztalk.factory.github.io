#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Schema.Annotation](Be.Stateless.BizTalk.Schema.Annotation.md 'Be.Stateless.BizTalk.Schema.Annotation')

## XPathExtractor Class

Denotes a context property whose value will be extracted from an [Microsoft.BizTalk.Message.Interop.IBaseMessagePart](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessagePart 'Microsoft.BizTalk.Message.Interop.IBaseMessagePart')'s payload while
being processed by the `Be.Stateless.BizTalk.Component.ContextPropertyExtractorComponent` pipeline
component.

```csharp
public class XPathExtractor : Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor,
System.IEquatable<Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor>
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [PropertyExtractor](PropertyExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor') &#129106; XPathExtractor

Derived  
&#8627; [QNameValueExtractor](QNameValueExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor')

Implements [System.IEquatable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.IEquatable-1 'System.IEquatable`1')[XPathExtractor](XPathExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.IEquatable-1 'System.IEquatable`1')

| Constructors | |
| :--- | :--- |
| [XPathExtractor(IMessageContextProperty, string, ExtractionMode)](XPathExtractor.XPathExtractor(IMessageContextProperty,string,ExtractionMode).md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.XPathExtractor(Be.Stateless.BizTalk.ContextProperties.IMessageContextProperty, string, Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode)') | |
| [XPathExtractor(XmlQualifiedName, string, ExtractionMode)](XPathExtractor.XPathExtractor(XmlQualifiedName,string,ExtractionMode).md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.XPathExtractor(System.Xml.XmlQualifiedName, string, Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode)') | |

| Properties | |
| :--- | :--- |
| [XPathExpression](XPathExtractor.XPathExpression.md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.XPathExpression') | |

| Methods | |
| :--- | :--- |
| [Equals(XPathExtractor)](XPathExtractor.Equals(XPathExtractor).md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.Equals(Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor)') | |
| [Equals(object)](XPathExtractor.Equals(object).md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.Equals(object)') | |
| [Execute(IBaseMessageContext, string, string)](XPathExtractor.Execute(IBaseMessageContext,string,string).md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.Execute(Microsoft.BizTalk.Message.Interop.IBaseMessageContext, string, string)') | |
| [GetHashCode()](XPathExtractor.GetHashCode().md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.GetHashCode()') | |
| [ToString()](XPathExtractor.ToString().md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.ToString()') | |
| [WriteXmlCore(XmlWriter)](XPathExtractor.WriteXmlCore(XmlWriter).md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.WriteXmlCore(System.Xml.XmlWriter)') | |

| Operators | |
| :--- | :--- |
| [operator ==(XPathExtractor, XPathExtractor)](XPathExtractor.operator(XPathExtractor,XPathExtractor).md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.op_Equality(Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor, Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor)') | |
| [operator !=(XPathExtractor, XPathExtractor)](XPathExtractor.operator!(XPathExtractor,XPathExtractor).md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.op_Inequality(Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor, Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor)') | |
