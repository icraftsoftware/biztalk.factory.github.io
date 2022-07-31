#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Component.Extensions](Be.Stateless.BizTalk.Component.Extensions.md 'Be.Stateless.BizTalk.Component.Extensions').[PipelineContextTrackingExtensions](PipelineContextTrackingExtensions.md 'Be.Stateless.BizTalk.Component.Extensions.PipelineContextTrackingExtensions')

## PipelineContextTrackingExtensions.GetActivityFactory(this IPipelineContext) Method

Tracking-activity factory for messaging-only activities.

```csharp
public static Be.Stateless.BizTalk.Activity.Tracking.Messaging.IActivityFactory GetActivityFactory(this Microsoft.BizTalk.Component.Interop.IPipelineContext pipelineContext);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Component.Extensions.PipelineContextTrackingExtensions.GetActivityFactory(thisMicrosoft.BizTalk.Component.Interop.IPipelineContext).pipelineContext'></a>

`pipelineContext` [Microsoft.BizTalk.Component.Interop.IPipelineContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPipelineContext 'Microsoft.BizTalk.Component.Interop.IPipelineContext')

The pipeline context from which messaging-only activities can be created.

#### Returns
[IActivityFactory](IActivityFactory.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.IActivityFactory')  
The activity factory.

### Remarks
The purpose of this factory is to make [Microsoft.BizTalk.Component.Interop.IPipelineContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPipelineContext 'Microsoft.BizTalk.Component.Interop.IPipelineContext') extension methods amenable to mocking, [http://blogs.clariusconsulting.net/kzu/how-to-mock-extension-methods/](http://blogs.clariusconsulting.net/kzu/how-to-mock-extension-methods/ 'http://blogs.clariusconsulting.net/kzu/how-to-mock-extension-methods/').

### See Also
- [http://blogs.clariusconsulting.net/kzu/how-extension-methods-ruined-unit-testing-and-oop-and-a-way-forward/](http://blogs.clariusconsulting.net/kzu/how-extension-methods-ruined-unit-testing-and-oop-and-a-way-forward/ 'http://blogs.clariusconsulting.net/kzu/how-extension-methods-ruined-unit-testing-and-oop-and-a-way-forward/')
- [http://blogs.clariusconsulting.net/kzu/making-extension-methods-amenable-to-mocking/](http://blogs.clariusconsulting.net/kzu/making-extension-methods-amenable-to-mocking/ 'http://blogs.clariusconsulting.net/kzu/making-extension-methods-amenable-to-mocking/')