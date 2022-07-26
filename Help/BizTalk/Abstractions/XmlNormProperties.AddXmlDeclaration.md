#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.ContextProperties](Be.Stateless.BizTalk.ContextProperties.md 'Be.Stateless.BizTalk.ContextProperties').[XmlNormProperties](XmlNormProperties.md 'Be.Stateless.BizTalk.ContextProperties.XmlNormProperties')

## XmlNormProperties.AddXmlDeclaration Field

Whether the XML Assembler pipeline component must preserve or remove the XML declaration.

```csharp
public static readonly MessageContextProperty<AddXMLDeclaration,bool> AddXmlDeclaration;
```

#### Field Value
[Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[XMLNORM.AddXMLDeclaration](https://docs.microsoft.com/en-us/dotnet/api/XMLNORM.AddXMLDeclaration 'XMLNORM.AddXMLDeclaration')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

### Remarks

If this option is set to `true` the the XML declaration will be added to the document. If the XML declaration
already existed, it will be overwritten.

If this option is set to `false`, no XML declaration will be added and any existing XML declaration will be
removed. The value of this property in the message context takes precedence over the value specified in Pipeline
Designer.

It defaults to `true`; the XML declaration is always added.

### See Also
- [https://github.com/MicrosoftDocs/biztalk-docs/blob/main/biztalk/core/xml-information-set-elements-in-the-xml-assembler-pipeline-component.md](https://github.com/MicrosoftDocs/biztalk-docs/blob/main/biztalk/core/xml-information-set-elements-in-the-xml-assembler-pipeline-component.md 'https://github.com/MicrosoftDocs/biztalk-docs/blob/main/biztalk/core/xml-information-set-elements-in-the-xml-assembler-pipeline-component.md')