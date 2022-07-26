#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language')

## IOperationCallbackSetup<TContract> Interface

Allows to setup the callback against [IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService') or [ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse') to be carried out
by the soap stub upon either the reception of some request message or the invocation of some SOAP action.

```csharp
public interface IOperationCallbackSetup<TContract> :
Be.Stateless.BizTalk.IFluentInterface
    where TContract : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup_TContract_.TContract'></a>

`TContract`

The the service contract to which belong operation that is being setup.

Derived  
&#8627; [IOperationCallSetup&lt;TContract&gt;](IOperationCallSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract>')

Implements [IFluentInterface](IFluentInterface.md 'Be.Stateless.BizTalk.IFluentInterface')

| Methods | |
| :--- | :--- |
| [Callback(Action)](IOperationCallbackSetup_TContract_.Callback(Action).md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup<TContract>.Callback(System.Action)') | Specifies a callback to invoke when the method is called. |
