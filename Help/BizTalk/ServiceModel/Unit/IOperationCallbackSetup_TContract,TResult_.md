#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language')

## IOperationCallbackSetup<TContract,TResult> Interface

Allows to setup the callback against [IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService') or [ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse') to be carried out
by the soap stub upon either the reception of some request message or the invocation of some SOAP action.

```csharp
public interface IOperationCallbackSetup<TContract,TResult> :
Be.Stateless.BizTalk.IFluentInterface
    where TContract : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup_TContract,TResult_.TContract'></a>

`TContract`

The the service contract to which belong operation that is being setup.

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup_TContract,TResult_.TResult'></a>

`TResult`

The type of the result the service contract's operation will produce.

Derived  
&#8627; [IOperationCallSetup&lt;TContract,TResult&gt;](IOperationCallSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract,TResult>')

Implements [IFluentInterface](IFluentInterface.md 'Be.Stateless.BizTalk.IFluentInterface')

| Methods | |
| :--- | :--- |
| [Callback(Action)](IOperationCallbackSetup_TContract,TResult_.Callback(Action).md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup<TContract,TResult>.Callback(System.Action)') | Specifies a callback to invoke when the method is called. |
