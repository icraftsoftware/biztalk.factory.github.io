#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Schema.Annotation](Be.Stateless.BizTalk.Schema.Annotation.md 'Be.Stateless.BizTalk.Schema.Annotation')

## QNameValueExtractor Class

Denotes a context property whose only the local part of a QName value will be extracted from an [Microsoft.BizTalk.Message.Interop.IBaseMessagePart](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessagePart 'Microsoft.BizTalk.Message.Interop.IBaseMessagePart')'s payload while being processed by the
`Be.Stateless.BizTalk.Component.ContextPropertyExtractorComponent` pipeline component.

```csharp
public class QNameValueExtractor : Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor,
System.IEquatable<Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor>
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [PropertyExtractor](PropertyExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor') &#129106; [XPathExtractor](XPathExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor') &#129106; QNameValueExtractor

Implements [System.IEquatable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.IEquatable-1 'System.IEquatable`1')[QNameValueExtractor](QNameValueExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.IEquatable-1 'System.IEquatable`1')

| Constructors | |
| :--- | :--- |
| [QNameValueExtractor(IMessageContextProperty, string, ExtractionMode, QNameValueExtractionMode)](QNameValueExtractor.QNameValueExtractor(IMessageContextProperty,string,ExtractionMode,QNameValueExtractionMode).md 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor.QNameValueExtractor(Be.Stateless.BizTalk.ContextProperties.IMessageContextProperty, string, Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode, Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractionMode)') | |
| [QNameValueExtractor(XmlQualifiedName, string, ExtractionMode, QNameValueExtractionMode)](QNameValueExtractor.QNameValueExtractor(XmlQualifiedName,string,ExtractionMode,QNameValueExtractionMode).md 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor.QNameValueExtractor(System.Xml.XmlQualifiedName, string, Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode, Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractionMode)') | |

| Properties | |
| :--- | :--- |
| [QNameValueExtractionMode](QNameValueExtractor.QNameValueExtractionMode.md 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor.QNameValueExtractionMode') | |

| Methods | |
| :--- | :--- |
| [Equals(QNameValueExtractor)](QNameValueExtractor.Equals(QNameValueExtractor).md 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor.Equals(Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor)') | |
| [Equals(object)](QNameValueExtractor.Equals(object).md 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor.Equals(object)') | |
| [Execute(IBaseMessageContext, string, string)](QNameValueExtractor.Execute(IBaseMessageContext,string,string).md 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor.Execute(Microsoft.BizTalk.Message.Interop.IBaseMessageContext, string, string)') | |
| [GetHashCode()](QNameValueExtractor.GetHashCode().md 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor.GetHashCode()') | |

| Operators | |
| :--- | :--- |
| [operator ==(QNameValueExtractor, QNameValueExtractor)](QNameValueExtractor.operator(QNameValueExtractor,QNameValueExtractor).md 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor.op_Equality(Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor, Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor)') | |
| [operator !=(QNameValueExtractor, QNameValueExtractor)](QNameValueExtractor.operator!(QNameValueExtractor,QNameValueExtractor).md 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor.op_Inequality(Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor, Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor)') | |
