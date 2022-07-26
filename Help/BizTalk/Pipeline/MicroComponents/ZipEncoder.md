#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent')

## ZipEncoder Class

Pipeline component which compresses the incoming data into a Zip Archive. The component wraps the message's original
stream in the zip-compressing stream [Be.Stateless.BizTalk.Stream.ZipOutputStream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream.ZipOutputStream 'Be.Stateless.BizTalk.Stream.ZipOutputStream').

```csharp
public class ZipEncoder :
Be.Stateless.BizTalk.MicroComponent.IMicroComponent
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ZipEncoder

Implements [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')

### Remarks
Zip-compress outbound message's body part stream.

### See Also
- [Be.Stateless.BizTalk.Stream.ZipOutputStream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream.ZipOutputStream 'Be.Stateless.BizTalk.Stream.ZipOutputStream')

| Methods | |
| :--- | :--- |
| [Execute(IPipelineContext, IBaseMessage)](ZipEncoder.Execute(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.MicroComponent.ZipEncoder.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
