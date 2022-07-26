#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent')

## MessageBodyStreamFactory Class

Micro component that replaces the [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') of the current message's [Microsoft.BizTalk.Message.Interop.IBaseMessage.BodyPart](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage.BodyPart 'Microsoft.BizTalk.Message.Interop.IBaseMessage.BodyPart') by a new one whose creation is delegated to either a contextual or statically
configurable [IMessageBodyStreamFactory](IMessageBodyStreamFactory.md 'Be.Stateless.BizTalk.MicroComponent.IMessageBodyStreamFactory') plugin.

```csharp
public class MessageBodyStreamFactory :
Be.Stateless.BizTalk.MicroComponent.IMicroComponent
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; MessageBodyStreamFactory

Implements [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')

| Properties | |
| :--- | :--- |
| [FactoryType](MessageBodyStreamFactory.FactoryType.md 'Be.Stateless.BizTalk.MicroComponent.MessageBodyStreamFactory.FactoryType') | The type of the [IMessageBodyStreamFactory](IMessageBodyStreamFactory.md 'Be.Stateless.BizTalk.MicroComponent.IMessageBodyStreamFactory') plugin that will be called to create the [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') of the message's [Microsoft.BizTalk.Message.Interop.IBaseMessage.BodyPart](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage.BodyPart 'Microsoft.BizTalk.Message.Interop.IBaseMessage.BodyPart'). |

| Methods | |
| :--- | :--- |
| [Execute(IPipelineContext, IBaseMessage)](MessageBodyStreamFactory.Execute(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.MicroComponent.MessageBodyStreamFactory.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
