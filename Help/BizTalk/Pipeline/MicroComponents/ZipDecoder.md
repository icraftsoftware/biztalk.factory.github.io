#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent')

## ZipDecoder Class

Pipeline component which decompresses the first entry of a Zip Archive. The component wraps the message's original
stream in the zip decompressing stream [Be.Stateless.BizTalk.Stream.ZipInputStream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream.ZipInputStream 'Be.Stateless.BizTalk.Stream.ZipInputStream').

```csharp
public class ZipDecoder :
Be.Stateless.BizTalk.MicroComponent.IMicroComponent
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ZipDecoder

Implements [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')

### Remarks
See [Be.Stateless.BizTalk.Stream.ZipInputStream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream.ZipInputStream 'Be.Stateless.BizTalk.Stream.ZipInputStream') for details on the Zip Archive format supported.

| Methods | |
| :--- | :--- |
| [Execute(IPipelineContext, IBaseMessage)](ZipDecoder.Execute(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.MicroComponent.ZipDecoder.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
