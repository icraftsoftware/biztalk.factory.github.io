#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.ContextProperties](Be.Stateless.BizTalk.ContextProperties.md 'Be.Stateless.BizTalk.ContextProperties').[XmlNormProperties](XmlNormProperties.md 'Be.Stateless.BizTalk.ContextProperties.XmlNormProperties')

## XmlNormProperties.AllowUnrecognizedMessage Field

Whether the XML Assembler and Disassembler pipeline components allows unrecognized Messages.

```csharp
public static readonly MessageContextProperty<AllowUnrecognizedMessage,bool> AllowUnrecognizedMessage;
```

#### Field Value
[Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[XMLNORM.AllowUnrecognizedMessage](https://docs.microsoft.com/en-us/dotnet/api/XMLNORM.AllowUnrecognizedMessage 'XMLNORM.AllowUnrecognizedMessage')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

### Remarks

It defaults to `false`.

### See Also
- [https://github.com/MicrosoftDocs/biztalk-docs/blob/main/biztalk/core/unrecognized-messages-in-the-xml-assembler-pipeline-component.md](https://github.com/MicrosoftDocs/biztalk-docs/blob/main/biztalk/core/unrecognized-messages-in-the-xml-assembler-pipeline-component.md 'https://github.com/MicrosoftDocs/biztalk-docs/blob/main/biztalk/core/unrecognized-messages-in-the-xml-assembler-pipeline-component.md')
- [https://github.com/MicrosoftDocs/biztalk-docs/blob/main/biztalk/core/unrecognized-messages-in-the-xml-disassembler-pipeline-component.md](https://github.com/MicrosoftDocs/biztalk-docs/blob/main/biztalk/core/unrecognized-messages-in-the-xml-disassembler-pipeline-component.md 'https://github.com/MicrosoftDocs/biztalk-docs/blob/main/biztalk/core/unrecognized-messages-in-the-xml-disassembler-pipeline-component.md')