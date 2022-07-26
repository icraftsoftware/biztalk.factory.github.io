#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language').[IOperationCallbackSetup&lt;TContract,TResult&gt;](IOperationCallbackSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup<TContract,TResult>')

## IOperationCallbackSetup<TContract,TResult>.Callback(Action) Method

Specifies a callback to invoke when the method is called.

```csharp
Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup<TContract,TResult> Callback(System.Action callback);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup_TContract,TResult_.Callback(System.Action).callback'></a>

`callback` [System.Action](https://docs.microsoft.com/en-us/dotnet/api/System.Action 'System.Action')

The callback method to invoke.

#### Returns
[Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup&lt;](IOperationAbortResponseSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup<TContract,TResult>')[TContract](IOperationCallbackSetup_TContract,TResult_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup_TContract,TResult_.TContract 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup<TContract,TResult>.TContract')[,](IOperationAbortResponseSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup<TContract,TResult>')[TResult](IOperationCallbackSetup_TContract,TResult_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup_TContract,TResult_.TResult 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup<TContract,TResult>.TResult')[&gt;](IOperationAbortResponseSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup<TContract,TResult>')  
An [IOperationResponseSetup&lt;TContract,TResult&gt;](IOperationResponseSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup<TContract,TResult>') object allowing to setup the actual response to return.