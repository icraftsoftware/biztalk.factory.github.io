#### [Be.Stateless.BizTalk.Process.NUnit](README.md 'README')
### [Be.Stateless.BizTalk.Unit](Be.Stateless.BizTalk.Unit.md 'Be.Stateless.BizTalk.Unit').[ProcessExtensions](ProcessExtensions.md 'Be.Stateless.BizTalk.Unit.ProcessExtensions')

## ProcessExtensions.SingleProcessingStep(this Process, Func<ProcessingStep,bool>) Method

```csharp
public static Be.Stateless.BizTalk.Activity.Monitoring.Model.ProcessingStep SingleProcessingStep(this Be.Stateless.BizTalk.Activity.Monitoring.Model.Process process, System.Func<Be.Stateless.BizTalk.Activity.Monitoring.Model.ProcessingStep,bool> predicate);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.ProcessExtensions.SingleProcessingStep(thisBe.Stateless.BizTalk.Activity.Monitoring.Model.Process,System.Func_Be.Stateless.BizTalk.Activity.Monitoring.Model.ProcessingStep,bool_).process'></a>

`process` [Be.Stateless.BizTalk.Activity.Monitoring.Model.Process](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Activity.Monitoring.Model.Process 'Be.Stateless.BizTalk.Activity.Monitoring.Model.Process')

<a name='Be.Stateless.BizTalk.Unit.ProcessExtensions.SingleProcessingStep(thisBe.Stateless.BizTalk.Activity.Monitoring.Model.Process,System.Func_Be.Stateless.BizTalk.Activity.Monitoring.Model.ProcessingStep,bool_).predicate'></a>

`predicate` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[Be.Stateless.BizTalk.Activity.Monitoring.Model.ProcessingStep](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Activity.Monitoring.Model.ProcessingStep 'Be.Stateless.BizTalk.Activity.Monitoring.Model.ProcessingStep')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')

#### Returns
[Be.Stateless.BizTalk.Activity.Monitoring.Model.ProcessingStep](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Activity.Monitoring.Model.ProcessingStep 'Be.Stateless.BizTalk.Activity.Monitoring.Model.ProcessingStep')