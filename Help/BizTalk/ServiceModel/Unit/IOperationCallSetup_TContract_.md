#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language')

## IOperationCallSetup<TContract> Interface

Allows to setup the various operations, like executing a callback or returning a specific response or aborting, that are
to be carried out by the [IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService') or [ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse') soap stub upon either the
reception of some request message or the invocation of some SOAP action.

```csharp
public interface IOperationCallSetup<TContract> :
Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup<TContract>,
Be.Stateless.BizTalk.IFluentInterface,
Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract>
    where TContract : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup_TContract_.TContract'></a>

`TContract`

The the service contract to which belong operation that is being setup.

Implements [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup&lt;](IOperationCallbackSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup<TContract>')[TContract](IOperationCallSetup_TContract_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup_TContract_.TContract 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract>.TContract')[&gt;](IOperationCallbackSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup<TContract>'), [IFluentInterface](IFluentInterface.md 'Be.Stateless.BizTalk.IFluentInterface'), [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup&lt;](IOperationAbortSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract>')[TContract](IOperationCallSetup_TContract_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup_TContract_.TContract 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract>.TContract')[&gt;](IOperationAbortSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract>')