#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language')

## IOperationAbortSetup<TContract> Interface

Allows to setup an abort to be carried out by the [IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService') or [ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse') soap
stub upon either the reception of some request message or the invocation of some SOAP action.

```csharp
public interface IOperationAbortSetup<TContract> :
Be.Stateless.BizTalk.IFluentInterface
    where TContract : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup_TContract_.TContract'></a>

`TContract`

The the service contract to which belong operation that is being setup.

Derived  
&#8627; [IOperationAbortResponseSetup&lt;TContract,TResult&gt;](IOperationAbortResponseSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup<TContract,TResult>')  
&#8627; [IOperationAbortSetup&lt;TContract,TResult&gt;](IOperationAbortSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract,TResult>')  
&#8627; [IOperationCallSetup&lt;TContract,TResult&gt;](IOperationCallSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract,TResult>')  
&#8627; [IOperationCallSetup&lt;TContract&gt;](IOperationCallSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract>')

Implements [IFluentInterface](IFluentInterface.md 'Be.Stateless.BizTalk.IFluentInterface')

| Methods | |
| :--- | :--- |
| [Aborts()](IOperationAbortSetup_TContract_.Aborts().md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract>.Aborts()') | Will setup the [IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService') soap stub to abort. |
