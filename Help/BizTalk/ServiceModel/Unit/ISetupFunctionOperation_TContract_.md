#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language')

## ISetupFunctionOperation<TContract> Interface

Allows to setup what the [IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService') or [ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse') soap stub has to perform upon
the invocation of some SOAP action, that is a service contract's operation.

```csharp
public interface ISetupFunctionOperation<TContract> :
Be.Stateless.BizTalk.IFluentInterface
    where TContract : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation_TContract_.TContract'></a>

`TContract`

The the service contract to which belong operation that is being setup.

Derived  
&#8627; [ISetupOperation&lt;TContract&gt;](ISetupOperation_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupOperation<TContract>')

Implements [IFluentInterface](IFluentInterface.md 'Be.Stateless.BizTalk.IFluentInterface')

| Methods | |
| :--- | :--- |
| [Setup&lt;TResult&gt;(Expression&lt;Func&lt;TContract,TResult&gt;&gt;)](ISetupFunctionOperation_TContract_.Setup_TResult_(Expression_Func_TContract,TResult__).md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation<TContract>.Setup<TResult>(System.Linq.Expressions.Expression<System.Func<TContract,TResult>>)') | Allows to setup what the [IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService') or [ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse') soap stub has to perform upon either the invocation of some SOAP action, that is service contract operation, that produces a result of type [TResult](ISetupFunctionOperation_TContract_.Setup_TResult_(Expression_Func_TContract,TResult__).md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation_TContract_.Setup_TResult_(System.Linq.Expressions.Expression_System.Func_TContract,TResult__).TResult 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation<TContract>.Setup<TResult>(System.Linq.Expressions.Expression<System.Func<TContract,TResult>>).TResult'). |
