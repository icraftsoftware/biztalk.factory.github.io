#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language')

## IOperationAbortResponseSetup<TContract,TResult> Interface

Allows to either setup the response that has to be returned, or an abort that has to be carried out by the [IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService') or [ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse') soap stub upon either the reception of some request message
or the invocation of some SOAP action.

```csharp
public interface IOperationAbortResponseSetup<TContract,TResult> :
Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract, TResult>,
Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract>,
Be.Stateless.BizTalk.IFluentInterface,
Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup<TContract, TResult>
    where TContract : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup_TContract,TResult_.TContract'></a>

`TContract`

The the service contract to which belong operation that is being setup.

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup_TContract,TResult_.TResult'></a>

`TResult`

The type of the result the service contract's operation will produce.

Derived  
&#8627; [IOperationCallSetup&lt;TContract,TResult&gt;](IOperationCallSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract,TResult>')

Implements [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup&lt;](IOperationAbortSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract,TResult>')[TContract](IOperationAbortResponseSetup_TContract,TResult_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup_TContract,TResult_.TContract 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup<TContract,TResult>.TContract')[,](IOperationAbortSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract,TResult>')[TResult](IOperationAbortResponseSetup_TContract,TResult_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup_TContract,TResult_.TResult 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup<TContract,TResult>.TResult')[&gt;](IOperationAbortSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract,TResult>'), [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup&lt;](IOperationAbortSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract>')[TContract](IOperationAbortResponseSetup_TContract,TResult_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup_TContract,TResult_.TContract 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup<TContract,TResult>.TContract')[&gt;](IOperationAbortSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract>'), [IFluentInterface](IFluentInterface.md 'Be.Stateless.BizTalk.IFluentInterface'), [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup&lt;](IOperationResponseSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup<TContract,TResult>')[TContract](IOperationAbortResponseSetup_TContract,TResult_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup_TContract,TResult_.TContract 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup<TContract,TResult>.TContract')[,](IOperationResponseSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup<TContract,TResult>')[TResult](IOperationAbortResponseSetup_TContract,TResult_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup_TContract,TResult_.TResult 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup<TContract,TResult>.TResult')[&gt;](IOperationResponseSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup<TContract,TResult>')