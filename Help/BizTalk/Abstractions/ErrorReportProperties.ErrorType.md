#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.ContextProperties](Be.Stateless.BizTalk.ContextProperties.md 'Be.Stateless.BizTalk.ContextProperties').[ErrorReportProperties](ErrorReportProperties.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties')

## ErrorReportProperties.ErrorType Field

Indicates the type of message that the error contains. This property always contains the value
FailedMessage, meaning that the error contains the original failed message.

```csharp
public static readonly MessageContextProperty<ErrorType,string> ErrorType;
```

#### Field Value
[Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[ErrorReport.ErrorType](https://docs.microsoft.com/en-us/dotnet/api/ErrorReport.ErrorType 'ErrorReport.ErrorType')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')