#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language').[ISetupActionOperation&lt;TContract&gt;](ISetupActionOperation_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupActionOperation<TContract>')

## ISetupActionOperation<TContract>.Setup(Expression<Action<TContract>>) Method

Allows to setup what the [IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService') or [ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse') soap stub has to perform
upon either the invocation of some SOAP action, that is service contract operation, that produces no result.

```csharp
Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract> Setup(System.Linq.Expressions.Expression<System.Action<TContract>> operation);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupActionOperation_TContract_.Setup(System.Linq.Expressions.Expression_System.Action_TContract__).operation'></a>

`operation` [System.Linq.Expressions.Expression&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Linq.Expressions.Expression-1 'System.Linq.Expressions.Expression`1')[System.Action&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')[TContract](ISetupActionOperation_TContract_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupActionOperation_TContract_.TContract 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupActionOperation<TContract>.TContract')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Linq.Expressions.Expression-1 'System.Linq.Expressions.Expression`1')

The expression tree denoting the operation contract for which a setup is being made.

#### Returns
[Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup&lt;](IOperationCallSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract>')[TContract](ISetupActionOperation_TContract_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupActionOperation_TContract_.TContract 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupActionOperation<TContract>.TContract')[&gt;](IOperationCallSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract>')  
An object that allows to record/setup the action to perform upon the invocation of some SOAP action, that is service
contract operation.