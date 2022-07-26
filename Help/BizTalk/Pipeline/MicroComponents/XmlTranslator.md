#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent')

## XmlTranslator Class

This component moves elements (and optionally attributes) from one namespace to another in the XML stream constituting
the body of the message.

```csharp
public class XmlTranslator :
Be.Stateless.BizTalk.MicroComponent.IMicroComponent
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; XmlTranslator

Implements [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')

| Properties | |
| :--- | :--- |
| [Encoding](XmlTranslator.Encoding.md 'Be.Stateless.BizTalk.MicroComponent.XmlTranslator.Encoding') | Encoding to use for output and, if Unicode, whether to emit a byte order mark. |
| [Modes](XmlTranslator.Modes.md 'Be.Stateless.BizTalk.MicroComponent.XmlTranslator.Modes') | |
| [Translations](XmlTranslator.Translations.md 'Be.Stateless.BizTalk.MicroComponent.XmlTranslator.Translations') | Set of XML translations to perform. |

| Methods | |
| :--- | :--- |
| [Execute(IPipelineContext, IBaseMessage)](XmlTranslator.Execute(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.MicroComponent.XmlTranslator.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
