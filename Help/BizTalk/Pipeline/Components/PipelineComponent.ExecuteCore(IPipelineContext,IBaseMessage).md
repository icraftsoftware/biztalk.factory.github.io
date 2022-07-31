#### [Be.Stateless.BizTalk.Pipeline.Components](README.md 'README')
### [Be.Stateless.BizTalk.Component](Be.Stateless.BizTalk.Component.md 'Be.Stateless.BizTalk.Component').[PipelineComponent](PipelineComponent.md 'Be.Stateless.BizTalk.Component.PipelineComponent')

## PipelineComponent.ExecuteCore(IPipelineContext, IBaseMessage) Method

Executes a pipeline component to process the input message and get the resulting message.

```csharp
protected internal abstract Microsoft.BizTalk.Message.Interop.IBaseMessage ExecuteCore(Microsoft.BizTalk.Component.Interop.IPipelineContext pipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage message);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Component.PipelineComponent.ExecuteCore(Microsoft.BizTalk.Component.Interop.IPipelineContext,Microsoft.BizTalk.Message.Interop.IBaseMessage).pipelineContext'></a>

`pipelineContext` [Microsoft.BizTalk.Component.Interop.IPipelineContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPipelineContext 'Microsoft.BizTalk.Component.Interop.IPipelineContext')

The [Microsoft.BizTalk.Component.Interop.IPipelineContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPipelineContext 'Microsoft.BizTalk.Component.Interop.IPipelineContext') that contains the current pipeline context.

<a name='Be.Stateless.BizTalk.Component.PipelineComponent.ExecuteCore(Microsoft.BizTalk.Component.Interop.IPipelineContext,Microsoft.BizTalk.Message.Interop.IBaseMessage).message'></a>

`message` [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage')

The [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage') that contains the message to process.

#### Returns
[Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage')  
The [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage') that contains the resulting message.