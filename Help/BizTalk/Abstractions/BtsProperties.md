#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.ContextProperties](Be.Stateless.BizTalk.ContextProperties.md 'Be.Stateless.BizTalk.ContextProperties')

## BtsProperties Class

System properties are mostly used internally by BizTalk Messaging Engine and its components. In general, changing the
values set by the engine for those properties is not recommended, because it may affect the execution logic of the
engine. However, there are a large number of properties that you can change.

```csharp
public abstract class BtsProperties
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; BtsProperties

### See Also
- [How to Use Message Context Properties](https://github.com/MicrosoftDocs/biztalk-docs/blob/master/biztalk/core/how-to-use-message-context-properties.md 'https://github.com/MicrosoftDocs/biztalk-docs/blob/master/biztalk/core/how-to-use-message-context-properties.md')

| Fields | |
| :--- | :--- |
| [AckRequired](BtsProperties.AckRequired.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.AckRequired') | |
| [ActualRetryCount](BtsProperties.ActualRetryCount.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.ActualRetryCount') | |
| [InboundTransportLocation](BtsProperties.InboundTransportLocation.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.InboundTransportLocation') | |
| [InboundTransportType](BtsProperties.InboundTransportType.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.InboundTransportType') | |
| [InterchangeID](BtsProperties.InterchangeID.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.InterchangeID') | |
| [IsDynamicSend](BtsProperties.IsDynamicSend.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.IsDynamicSend') | |
| [IsRequestResponse](BtsProperties.IsRequestResponse.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.IsRequestResponse') | |
| [IsSolicitResponse](BtsProperties.IsSolicitResponse.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.IsSolicitResponse') | |
| [MessageDestination](BtsProperties.MessageDestination.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.MessageDestination') | |
| [MessageID](BtsProperties.MessageID.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.MessageID') | |
| [MessageType](BtsProperties.MessageType.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.MessageType') | |
| [Operation](BtsProperties.Operation.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.Operation') | |
| [OutboundTransportCLSID](BtsProperties.OutboundTransportCLSID.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.OutboundTransportCLSID') | |
| [OutboundTransportLocation](BtsProperties.OutboundTransportLocation.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.OutboundTransportLocation') | |
| [OutboundTransportType](BtsProperties.OutboundTransportType.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.OutboundTransportType') | |
| [ReceiveLocationName](BtsProperties.ReceiveLocationName.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.ReceiveLocationName') | |
| [ReceivePipelineConfig](BtsProperties.ReceivePipelineConfig.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.ReceivePipelineConfig') | |
| [ReceivePortName](BtsProperties.ReceivePortName.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.ReceivePortName') | |
| [RetryCount](BtsProperties.RetryCount.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.RetryCount') | |
| [RetryInterval](BtsProperties.RetryInterval.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.RetryInterval') | |
| [RouteMessageOnFailure](BtsProperties.RouteMessageOnFailure.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.RouteMessageOnFailure') | |
| [SchemaStrongName](BtsProperties.SchemaStrongName.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.SchemaStrongName') | |
| [SendPortName](BtsProperties.SendPortName.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.SendPortName') | |
| [SuppressRoutingFailureDiagnosticInfo](BtsProperties.SuppressRoutingFailureDiagnosticInfo.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.SuppressRoutingFailureDiagnosticInfo') | |
| [SuspendMessageOnRoutingFailure](BtsProperties.SuspendMessageOnRoutingFailure.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.SuspendMessageOnRoutingFailure') | |
| [TransmitWorkID](BtsProperties.TransmitWorkID.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.TransmitWorkID') | |
| [WasSolicitResponse](BtsProperties.WasSolicitResponse.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.WasSolicitResponse') | |
