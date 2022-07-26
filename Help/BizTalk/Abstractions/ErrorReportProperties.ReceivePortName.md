#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.ContextProperties](Be.Stateless.BizTalk.ContextProperties.md 'Be.Stateless.BizTalk.ContextProperties').[ErrorReportProperties](ErrorReportProperties.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties')

## ErrorReportProperties.ReceivePortName Field

Name of the receive port where the failure happened.

```csharp
public static readonly MessageContextProperty<ReceivePortName,string> ReceivePortName;
```

#### Field Value
[Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[ErrorReport.ReceivePortName](https://docs.microsoft.com/en-us/dotnet/api/ErrorReport.ReceivePortName 'ErrorReport.ReceivePortName')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

### Remarks
Promoted if the failure happened during inbound processing (in a receive port).
Not promoted if the failure happened in a send port.