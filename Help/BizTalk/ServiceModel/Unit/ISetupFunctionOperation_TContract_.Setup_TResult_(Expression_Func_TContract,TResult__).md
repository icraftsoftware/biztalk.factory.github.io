#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language').[ISetupFunctionOperation&lt;TContract&gt;](ISetupFunctionOperation_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation<TContract>')

## ISetupFunctionOperation<TContract>.Setup<TResult>(Expression<Func<TContract,TResult>>) Method

Allows to setup what the [IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService') or [ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse') soap stub has to perform
upon either the invocation of some SOAP action, that is service contract operation, that produces a result of type
[TResult](ISetupFunctionOperation_TContract_.Setup_TResult_(Expression_Func_TContract,TResult__).md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation_TContract_.Setup_TResult_(System.Linq.Expressions.Expression_System.Func_TContract,TResult__).TResult 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation<TContract>.Setup<TResult>(System.Linq.Expressions.Expression<System.Func<TContract,TResult>>).TResult').

```csharp
Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract,TResult> Setup<TResult>(System.Linq.Expressions.Expression<System.Func<TContract,TResult>> operation);
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation_TContract_.Setup_TResult_(System.Linq.Expressions.Expression_System.Func_TContract,TResult__).TResult'></a>

`TResult`

The type of the result produced by the [operation](ISetupFunctionOperation_TContract_.Setup_TResult_(Expression_Func_TContract,TResult__).md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation_TContract_.Setup_TResult_(System.Linq.Expressions.Expression_System.Func_TContract,TResult__).operation 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation<TContract>.Setup<TResult>(System.Linq.Expressions.Expression<System.Func<TContract,TResult>>).operation') being performed.
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation_TContract_.Setup_TResult_(System.Linq.Expressions.Expression_System.Func_TContract,TResult__).operation'></a>

`operation` [System.Linq.Expressions.Expression&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Linq.Expressions.Expression-1 'System.Linq.Expressions.Expression`1')[System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[TContract](ISetupFunctionOperation_TContract_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation_TContract_.TContract 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation<TContract>.TContract')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[TResult](ISetupFunctionOperation_TContract_.Setup_TResult_(Expression_Func_TContract,TResult__).md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation_TContract_.Setup_TResult_(System.Linq.Expressions.Expression_System.Func_TContract,TResult__).TResult 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation<TContract>.Setup<TResult>(System.Linq.Expressions.Expression<System.Func<TContract,TResult>>).TResult')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Linq.Expressions.Expression-1 'System.Linq.Expressions.Expression`1')

The expression tree denoting the operation contract for which a setup is being made.

#### Returns
[Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup&lt;](IOperationCallSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract,TResult>')[TContract](ISetupFunctionOperation_TContract_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation_TContract_.TContract 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation<TContract>.TContract')[,](IOperationCallSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract,TResult>')[TResult](ISetupFunctionOperation_TContract_.Setup_TResult_(Expression_Func_TContract,TResult__).md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation_TContract_.Setup_TResult_(System.Linq.Expressions.Expression_System.Func_TContract,TResult__).TResult 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation<TContract>.Setup<TResult>(System.Linq.Expressions.Expression<System.Func<TContract,TResult>>).TResult')[&gt;](IOperationCallSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract,TResult>')  
An object that allows to record/setup the action to perform upon the invocation of some SOAP action, that is service
contract operation.