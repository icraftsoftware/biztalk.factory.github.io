#### [Be.Stateless.BizTalk.Process.NUnit](README.md 'README')
### [Be.Stateless.BizTalk.Unit](Be.Stateless.BizTalk.Unit.md 'Be.Stateless.BizTalk.Unit').[ProcessExtensions](ProcessExtensions.md 'Be.Stateless.BizTalk.Unit.ProcessExtensions')

## ProcessExtensions.SingleMessagingStep(this Process, Func<MessagingStep,bool>) Method

```csharp
public static Be.Stateless.BizTalk.Activity.Monitoring.Model.MessagingStep SingleMessagingStep(this Be.Stateless.BizTalk.Activity.Monitoring.Model.Process process, System.Func<Be.Stateless.BizTalk.Activity.Monitoring.Model.MessagingStep,bool> predicate);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.ProcessExtensions.SingleMessagingStep(thisBe.Stateless.BizTalk.Activity.Monitoring.Model.Process,System.Func_Be.Stateless.BizTalk.Activity.Monitoring.Model.MessagingStep,bool_).process'></a>

`process` [Be.Stateless.BizTalk.Activity.Monitoring.Model.Process](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Activity.Monitoring.Model.Process 'Be.Stateless.BizTalk.Activity.Monitoring.Model.Process')

<a name='Be.Stateless.BizTalk.Unit.ProcessExtensions.SingleMessagingStep(thisBe.Stateless.BizTalk.Activity.Monitoring.Model.Process,System.Func_Be.Stateless.BizTalk.Activity.Monitoring.Model.MessagingStep,bool_).predicate'></a>

`predicate` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[Be.Stateless.BizTalk.Activity.Monitoring.Model.MessagingStep](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Activity.Monitoring.Model.MessagingStep 'Be.Stateless.BizTalk.Activity.Monitoring.Model.MessagingStep')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')

#### Returns
[Be.Stateless.BizTalk.Activity.Monitoring.Model.MessagingStep](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Activity.Monitoring.Model.MessagingStep 'Be.Stateless.BizTalk.Activity.Monitoring.Model.MessagingStep')