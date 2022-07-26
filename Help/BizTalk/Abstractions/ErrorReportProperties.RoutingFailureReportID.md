#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.ContextProperties](Be.Stateless.BizTalk.ContextProperties.md 'Be.Stateless.BizTalk.ContextProperties').[ErrorReportProperties](ErrorReportProperties.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties')

## ErrorReportProperties.RoutingFailureReportID Field

This property provides the ID of the routing failure report that BizTalk Server generates when there
is a routing failure. A routing failure report is a special message that BizTalk Server generates
and suspends. This message does not have a body, but it has the context of the failed message. Using
this ID, an error-handling orchestration or a send port can query the MessageBox database and
process the routing failure report. For example, an orchestration may want to terminate the routing
failure report after it gets the failed message.

```csharp
public static readonly MessageContextProperty<RoutingFailureReportID,string> RoutingFailureReportID;
```

#### Field Value
[Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[ErrorReport.RoutingFailureReportID](https://docs.microsoft.com/en-us/dotnet/api/ErrorReport.RoutingFailureReportID 'ErrorReport.RoutingFailureReportID')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')