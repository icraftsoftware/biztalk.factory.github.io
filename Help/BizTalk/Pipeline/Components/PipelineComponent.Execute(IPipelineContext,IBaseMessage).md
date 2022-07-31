#### [Be.Stateless.BizTalk.Pipeline.Components](README.md 'README')
### [Be.Stateless.BizTalk.Component](Be.Stateless.BizTalk.Component.md 'Be.Stateless.BizTalk.Component').[PipelineComponent](PipelineComponent.md 'Be.Stateless.BizTalk.Component.PipelineComponent')

## PipelineComponent.Execute(IPipelineContext, IBaseMessage) Method

Executes a pipeline component to process the input message and get the resulting message.

```csharp
public Microsoft.BizTalk.Message.Interop.IBaseMessage Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext pipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage message);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Component.PipelineComponent.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext,Microsoft.BizTalk.Message.Interop.IBaseMessage).pipelineContext'></a>

`pipelineContext` [Microsoft.BizTalk.Component.Interop.IPipelineContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPipelineContext 'Microsoft.BizTalk.Component.Interop.IPipelineContext')

The [Microsoft.BizTalk.Component.Interop.IPipelineContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPipelineContext 'Microsoft.BizTalk.Component.Interop.IPipelineContext') that contains the current pipeline context.

<a name='Be.Stateless.BizTalk.Component.PipelineComponent.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext,Microsoft.BizTalk.Message.Interop.IBaseMessage).message'></a>

`message` [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage')

The [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage') that contains the message to process.

Implements [Execute(IPipelineContext, IBaseMessage)](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IComponent.Execute#Microsoft_BizTalk_Component_Interop_IComponent_Execute_Microsoft_BizTalk_Component_Interop_IPipelineContext,Microsoft_BizTalk_Message_Interop_IBaseMessage_ 'Microsoft.BizTalk.Component.Interop.IComponent.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext,Microsoft.BizTalk.Message.Interop.IBaseMessage)')

#### Returns
[Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage')  
The [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage') that contains the resulting message.