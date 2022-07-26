#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language').[IOperationCallbackSetup&lt;TContract&gt;](IOperationCallbackSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup<TContract>')

## IOperationCallbackSetup<TContract>.Callback(Action) Method

Specifies a callback to invoke when the method is called.

```csharp
Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract> Callback(System.Action callback);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup_TContract_.Callback(System.Action).callback'></a>

`callback` [System.Action](https://docs.microsoft.com/en-us/dotnet/api/System.Action 'System.Action')

The callback method to invoke.

#### Returns
[Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup&lt;](IOperationAbortSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract>')[TContract](IOperationCallbackSetup_TContract_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup_TContract_.TContract 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup<TContract>.TContract')[&gt;](IOperationAbortSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract>')  
An [IOperationResponseSetup&lt;TContract,TResult&gt;](IOperationResponseSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup<TContract,TResult>') object allowing to setup the actual response to return.