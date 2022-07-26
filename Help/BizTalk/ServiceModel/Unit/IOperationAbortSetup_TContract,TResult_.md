#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language')

## IOperationAbortSetup<TContract,TResult> Interface

Allows to setup an abort to be carried out by the [IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService') or [ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse') soap
stub upon either the reception of some request message or the invocation of some SOAP action.

```csharp
public interface IOperationAbortSetup<TContract,TResult> :
Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract>,
Be.Stateless.BizTalk.IFluentInterface
    where TContract : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup_TContract,TResult_.TContract'></a>

`TContract`

The the service contract to which belong operation that is being setup.

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup_TContract,TResult_.TResult'></a>

`TResult`

Derived  
&#8627; [IOperationAbortResponseSetup&lt;TContract,TResult&gt;](IOperationAbortResponseSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup<TContract,TResult>')  
&#8627; [IOperationCallSetup&lt;TContract,TResult&gt;](IOperationCallSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract,TResult>')

Implements [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup&lt;](IOperationAbortSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract>')[TContract](IOperationAbortSetup_TContract,TResult_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup_TContract,TResult_.TContract 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract,TResult>.TContract')[&gt;](IOperationAbortSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract>'), [IFluentInterface](IFluentInterface.md 'Be.Stateless.BizTalk.IFluentInterface')