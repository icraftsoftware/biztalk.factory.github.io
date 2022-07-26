#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.ContextProperties](Be.Stateless.BizTalk.ContextProperties.md 'Be.Stateless.BizTalk.ContextProperties')

## ErrorReportProperties Class

The properties that are promoted to the context of an error message.

```csharp
public static class ErrorReportProperties
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ErrorReportProperties

### See Also
- [http://msdn.microsoft.com/en-us/library/aa578516(BTS.10).aspx](http://msdn.microsoft.com/en-us/library/aa578516(BTS.10).aspx 'http://msdn.microsoft.com/en-us/library/aa578516(BTS.10).aspx')
- [http://support.microsoft.com/kb/944532](http://support.microsoft.com/kb/944532 'http://support.microsoft.com/kb/944532')

| Fields | |
| :--- | :--- |
| [Description](ErrorReportProperties.Description.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties.Description') | Error description. Same diagnostic text as is written to the Application Event Log regarding this messaging failure. |
| [ErrorType](ErrorReportProperties.ErrorType.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties.ErrorType') | Indicates the type of message that the error contains. This property always contains the value FailedMessage, meaning that the error contains the original failed message. |
| [FailureAdapter](ErrorReportProperties.FailureAdapter.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties.FailureAdapter') | Adapter that is associated with the error that generates the error report. |
| [FailureCode](ErrorReportProperties.FailureCode.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties.FailureCode') | Error code. A hexadecimal value that is reported in the BizTalk Server Administration console. |
| [FailureInstanceID](ErrorReportProperties.FailureInstanceID.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties.FailureInstanceID') | Instance ID of the message or instance that has an error. |
| [FailureMessageID](ErrorReportProperties.FailureMessageID.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties.FailureMessageID') | Message ID of the message that has an error. |
| [FailureTime](ErrorReportProperties.FailureTime.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties.FailureTime') | Current UTC time when the error report is generated. |
| [InboundTransportLocation](ErrorReportProperties.InboundTransportLocation.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties.InboundTransportLocation') | URI of the receive location where the failure happened. |
| [MessageType](ErrorReportProperties.MessageType.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties.MessageType') | Message type of failed message, or empty if message type is indeterminate. |
| [OutboundTransportLocation](ErrorReportProperties.OutboundTransportLocation.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties.OutboundTransportLocation') | URI of the send location where the failure happened. |
| [ProcessingServer](ErrorReportProperties.ProcessingServer.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties.ProcessingServer') | Name of the server where the failure happened. |
| [ReceivePortName](ErrorReportProperties.ReceivePortName.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties.ReceivePortName') | Name of the receive port where the failure happened. |
| [RoutingFailureReportID](ErrorReportProperties.RoutingFailureReportID.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties.RoutingFailureReportID') | This property provides the ID of the routing failure report that BizTalk Server generates when there is a routing failure. A routing failure report is a special message that BizTalk Server generates and suspends. This message does not have a body, but it has the context of the failed message. Using this ID, an error-handling orchestration or a send port can query the MessageBox database and process the routing failure report. For example, an orchestration may want to terminate the routing failure report after it gets the failed message. |
| [SendPortName](ErrorReportProperties.SendPortName.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties.SendPortName') | Name of the send port where the failure happened. |
