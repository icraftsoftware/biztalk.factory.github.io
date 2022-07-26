#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent')

## XsltRunner Class

Pipeline component that applies an XSL Transformation on messages along their way in the pipeline.

```csharp
public class XsltRunner :
Be.Stateless.BizTalk.MicroComponent.IMicroComponent
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; XsltRunner

Implements [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')

### Remarks
Contrary to maps statically-configured at the receive or send port level, [XsltRunner](XsltRunner.md 'Be.Stateless.BizTalk.MicroComponent.XsltRunner') allows for:
- the transform to be dynamically chosen;
- the transform to be executed anywhere in the pipeline. This is particularly interesting, as we can choose to place
              it before or after an XML assembler/disassembler;
- the execution to be conditional;
- arguments to be dynamically supplied to the transform.

| Properties | |
| :--- | :--- |
| [Encoding](XsltRunner.Encoding.md 'Be.Stateless.BizTalk.MicroComponent.XsltRunner.Encoding') | Encoding to use for output and, if Unicode, whether to emit a byte order mark. |
| [MapType](XsltRunner.MapType.md 'Be.Stateless.BizTalk.MicroComponent.XsltRunner.MapType') | The type name of the BizTalk Map to apply to the message. |

| Methods | |
| :--- | :--- |
| [Execute(IPipelineContext, IBaseMessage)](XsltRunner.Execute(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.MicroComponent.XsltRunner.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
