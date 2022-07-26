#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.ContextProperties](Be.Stateless.BizTalk.ContextProperties.md 'Be.Stateless.BizTalk.ContextProperties').[ErrorReportProperties](ErrorReportProperties.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties')

## ErrorReportProperties.OutboundTransportLocation Field

URI of the send location where the failure happened.

```csharp
public static readonly MessageContextProperty<OutboundTransportLocation,string> OutboundTransportLocation;
```

#### Field Value
[Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[ErrorReport.OutboundTransportLocation](https://docs.microsoft.com/en-us/dotnet/api/ErrorReport.OutboundTransportLocation 'ErrorReport.OutboundTransportLocation')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

### Remarks
Promoted if the failure happened during outbound processing (in a send port).
Not promoted if the failure happened in a receive port.