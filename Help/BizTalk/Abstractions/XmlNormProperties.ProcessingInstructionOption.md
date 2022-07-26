#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.ContextProperties](Be.Stateless.BizTalk.ContextProperties.md 'Be.Stateless.BizTalk.ContextProperties').[XmlNormProperties](XmlNormProperties.md 'Be.Stateless.BizTalk.ContextProperties.XmlNormProperties')

## XmlNormProperties.ProcessingInstructionOption Field

How to handle the processing instructions specified by [ProcessingInstruction](XmlNormProperties.ProcessingInstruction.md 'Be.Stateless.BizTalk.ContextProperties.XmlNormProperties.ProcessingInstruction').

```csharp
public static readonly MessageContextProperty<ProcessingInstructionOption,int> ProcessingInstructionOption;
```

#### Field Value
[Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[XMLNORM.ProcessingInstructionOption](https://docs.microsoft.com/en-us/dotnet/api/XMLNORM.ProcessingInstructionOption 'XMLNORM.ProcessingInstructionOption')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

### Remarks

[ProcessingInstructionOption](XmlNormProperties.ProcessingInstructionOption.md 'Be.Stateless.BizTalk.ContextProperties.XmlNormProperties.ProcessingInstructionOption') has three possible values:
            

|Value|
|-|
|New processing instructions from the XML Assembler are appended to the processing instructions at the beginning of the document.|
|New processing instructions from the XML Assembler overwrite existing processing instructions at the beginning of the document.|
|Processing instructions at the beginning of the document are removed.|

### See Also
- [https://github.com/MicrosoftDocs/biztalk-docs/blob/main/biztalk/core/processing-instructions-in-the-xml-assembler-pipeline-component.md](https://github.com/MicrosoftDocs/biztalk-docs/blob/main/biztalk/core/processing-instructions-in-the-xml-assembler-pipeline-component.md 'https://github.com/MicrosoftDocs/biztalk-docs/blob/main/biztalk/core/processing-instructions-in-the-xml-assembler-pipeline-component.md')