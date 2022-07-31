#### [Be.Stateless.BizTalk.Batching](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent')

## EnvelopeBuilder Class

Pipeline component that transforms a [Be.Stateless.BizTalk.Schemas.Xml.Batch.Content](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schemas.Xml.Batch.Content 'Be.Stateless.BizTalk.Schemas.Xml.Batch.Content') with all its parts into its affiliated envelope.

```csharp
public class EnvelopeBuilder : Be.Stateless.BizTalk.MicroComponent.XsltRunner
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.BizTalk.MicroComponent.XsltRunner](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.MicroComponent.XsltRunner 'Be.Stateless.BizTalk.MicroComponent.XsltRunner') &#129106; EnvelopeBuilder

### Remarks
It is meant to be used in the receive pipeline of the receive location that polls for batches to release.

| Methods | |
| :--- | :--- |
| [Execute(IPipelineContext, IBaseMessage)](EnvelopeBuilder.Execute(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.MicroComponent.EnvelopeBuilder.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
