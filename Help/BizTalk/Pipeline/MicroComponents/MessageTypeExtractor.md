#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent')

## MessageTypeExtractor Class

Probe the current message for its type and write it in the [BizTalkFactoryProperties.MessageType](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.MessageType 'Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.MessageType') context property.

```csharp
public class MessageTypeExtractor :
Be.Stateless.BizTalk.MicroComponent.IMicroComponent
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; MessageTypeExtractor

Implements [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')

### Remarks
This component will always probe the current message for its type and will consequently always install a [Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream 'Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream') around the current message's body part stream.

| Methods | |
| :--- | :--- |
| [Execute(IPipelineContext, IBaseMessage)](MessageTypeExtractor.Execute(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.MicroComponent.MessageTypeExtractor.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
