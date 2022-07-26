#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent')

## TransportRetriesDisabler Class

Prevent Microsoft BizTalk Server's SendPort Transport from performing any retries to send the message in case of
failures provided the property [Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.DisableTransportRetries](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.DisableTransportRetries 'Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.DisableTransportRetries') is present in the
message's context and has a value of `true`.

```csharp
public class TransportRetriesDisabler :
Be.Stateless.BizTalk.MicroComponent.IMicroComponent
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; TransportRetriesDisabler

Implements [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')

| Methods | |
| :--- | :--- |
| [Execute(IPipelineContext, IBaseMessage)](TransportRetriesDisabler.Execute(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.MicroComponent.TransportRetriesDisabler.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
