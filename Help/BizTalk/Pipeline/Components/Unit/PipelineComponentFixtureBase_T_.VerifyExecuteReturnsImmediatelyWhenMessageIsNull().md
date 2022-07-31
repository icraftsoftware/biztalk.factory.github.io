#### [Be.Stateless.BizTalk.Pipeline.Components.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Component](Be.Stateless.BizTalk.Unit.Component.md 'Be.Stateless.BizTalk.Unit.Component').[PipelineComponentFixtureBase&lt;T&gt;](PipelineComponentFixtureBase_T_.md 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase<T>')

## PipelineComponentFixtureBase<T>.VerifyExecuteReturnsImmediatelyWhenMessageIsNull() Method

Ensure [Be.Stateless.BizTalk.Component.PipelineComponent](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Component.PipelineComponent 'Be.Stateless.BizTalk.Component.PipelineComponent')-derived class does not break the implementation of the [Microsoft.BizTalk.Component.Interop.IComponent.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext,Microsoft.BizTalk.Message.Interop.IBaseMessage)](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IComponent.Execute#Microsoft_BizTalk_Component_Interop_IComponent_Execute_Microsoft_BizTalk_Component_Interop_IPipelineContext,Microsoft_BizTalk_Message_Interop_IBaseMessage_ 'Microsoft.BizTalk.Component.Interop.IComponent.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext,Microsoft.BizTalk.Message.Interop.IBaseMessage)') method from its base class.

```csharp
protected void VerifyExecuteReturnsImmediatelyWhenMessageIsNull();
```