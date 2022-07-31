#### [Be.Stateless.BizTalk.Schemas](README.md 'README')
### [Be.Stateless.BizTalk.ContextProperties.Subscribable](Be.Stateless.BizTalk.ContextProperties.Subscribable.md 'Be.Stateless.BizTalk.ContextProperties.Subscribable')

## BizTalkFactoryProperties Class

```csharp
public abstract class BizTalkFactoryProperties : Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties 'Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties') &#129106; BizTalkFactoryProperties

| Fields | |
| :--- | :--- |
| [CorrelationId](BizTalkFactoryProperties.CorrelationId.md 'Be.Stateless.BizTalk.ContextProperties.Subscribable.BizTalkFactoryProperties.CorrelationId') | |
| [EnvironmentTag](BizTalkFactoryProperties.EnvironmentTag.md 'Be.Stateless.BizTalk.ContextProperties.Subscribable.BizTalkFactoryProperties.EnvironmentTag') | To be used when one application has to be connected to several distinct sets of interacting parties and cannot leak messages from one set of parties into another. In concrete terms, to be used in pub/sub of messages in order to keep them strictly insulated within an individual set of such interacting parties. |
| [ReceiverName](BizTalkFactoryProperties.ReceiverName.md 'Be.Stateless.BizTalk.ContextProperties.Subscribable.BizTalkFactoryProperties.ReceiverName') | Name of the intended receiver of the current message. |
| [SenderName](BizTalkFactoryProperties.SenderName.md 'Be.Stateless.BizTalk.ContextProperties.Subscribable.BizTalkFactoryProperties.SenderName') | Name of the initiating sender of the current message. |
