#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.ContextProperties](Be.Stateless.BizTalk.ContextProperties.md 'Be.Stateless.BizTalk.ContextProperties').[ErrorReportProperties](ErrorReportProperties.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties')

## ErrorReportProperties.InboundTransportLocation Field

URI of the receive location where the failure happened.

```csharp
public static readonly MessageContextProperty<InboundTransportLocation,string> InboundTransportLocation;
```

#### Field Value
[Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[ErrorReport.InboundTransportLocation](https://docs.microsoft.com/en-us/dotnet/api/ErrorReport.InboundTransportLocation 'ErrorReport.InboundTransportLocation')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

### Remarks
Promoted if the failure happened during inbound processing (in a receive port).
Not promoted if the failure happened in a send port.