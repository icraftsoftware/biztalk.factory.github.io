#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent')

## SBMessagingContextPropagator Class

Propagates message type and correlation id over inbound and outbound Azure ServiceBus queues.

```csharp
public class SBMessagingContextPropagator :
Be.Stateless.BizTalk.MicroComponent.IMicroComponent
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; SBMessagingContextPropagator

Implements [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')

### Remarks

For inbound messages, [SBMessagingProperties.CorrelationId](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.SBMessagingProperties.CorrelationId 'Be.Stateless.BizTalk.ContextProperties.SBMessagingProperties.CorrelationId'), if any,
is promoted into BizTalk Server message context as `BizTalkFactoryProperties.CorrelationId` property.

For outbound messages, `BizTalkFactoryProperties.CorrelationId` and [BtsProperties.MessageType](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.BtsProperties.MessageType 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.MessageType'), if any, are respectively propagated as
[SBMessagingProperties.CorrelationId](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.SBMessagingProperties.CorrelationId 'Be.Stateless.BizTalk.ContextProperties.SBMessagingProperties.CorrelationId')
and `MessageType` in namespace declared by `SB-Messaging` adapter's [SBMessaging.CustomBrokeredMessagePropertyNamespace](https://docs.microsoft.com/en-us/dotnet/api/SBMessaging.CustomBrokeredMessagePropertyNamespace 'SBMessaging.CustomBrokeredMessagePropertyNamespace') configuration property.

| Methods | |
| :--- | :--- |
| [Execute(IPipelineContext, IBaseMessage)](SBMessagingContextPropagator.Execute(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.MicroComponent.SBMessagingContextPropagator.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
