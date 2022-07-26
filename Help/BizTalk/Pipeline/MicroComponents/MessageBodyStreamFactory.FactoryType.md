#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent').[MessageBodyStreamFactory](MessageBodyStreamFactory.md 'Be.Stateless.BizTalk.MicroComponent.MessageBodyStreamFactory')

## MessageBodyStreamFactory.FactoryType Property

The type of the [IMessageBodyStreamFactory](IMessageBodyStreamFactory.md 'Be.Stateless.BizTalk.MicroComponent.IMessageBodyStreamFactory') plugin that will be called to create the [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') of the message's [Microsoft.BizTalk.Message.Interop.IBaseMessage.BodyPart](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage.BodyPart 'Microsoft.BizTalk.Message.Interop.IBaseMessage.BodyPart').

```csharp
public System.Type FactoryType { get; set; }
```

#### Property Value
[System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')