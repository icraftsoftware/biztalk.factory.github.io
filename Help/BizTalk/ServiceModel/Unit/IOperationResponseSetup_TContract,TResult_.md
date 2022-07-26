#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language')

## IOperationResponseSetup<TContract,TResult> Interface

Allows to setup the response that has to be returned by the [IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService') or [ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse') soap stub upon either the reception of some request message or the invocation of some SOAP
action.

```csharp
public interface IOperationResponseSetup<TContract,TResult> :
Be.Stateless.BizTalk.IFluentInterface
    where TContract : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup_TContract,TResult_.TContract'></a>

`TContract`

The the service contract to which belong operation that is being setup.

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup_TContract,TResult_.TResult'></a>

`TResult`

The type of the result the service contract's operation will produce.

Derived  
&#8627; [IOperationAbortResponseSetup&lt;TContract,TResult&gt;](IOperationAbortResponseSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup<TContract,TResult>')  
&#8627; [IOperationCallSetup&lt;TContract,TResult&gt;](IOperationCallSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract,TResult>')

Implements [IFluentInterface](IFluentInterface.md 'Be.Stateless.BizTalk.IFluentInterface')

| Methods | |
| :--- | :--- |
| [Returns(string)](IOperationResponseSetup_TContract,TResult_.Returns(string).md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup<TContract,TResult>.Returns(string)') | Will setup the content of the [file](IOperationResponseSetup_TContract,TResult_.Returns(string).md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup_TContract,TResult_.Returns(string).file 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup<TContract,TResult>.Returns(string).file') as the response's body stream. |
| [Returns(Stream)](IOperationResponseSetup_TContract,TResult_.Returns(Stream).md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup<TContract,TResult>.Returns(System.IO.Stream)') | Will setup the [stream](IOperationResponseSetup_TContract,TResult_.Returns(Stream).md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup_TContract,TResult_.Returns(System.IO.Stream).stream 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup<TContract,TResult>.Returns(System.IO.Stream).stream') as the response's body stream. |
