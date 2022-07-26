#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language')

## ISetupActionOperation<TContract> Interface

Allows to setup what the [IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService') or [ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse') soap stub has to perform upon
the invocation of some SOAP action, that is a service contract's operation.

```csharp
public interface ISetupActionOperation<TContract> :
Be.Stateless.BizTalk.IFluentInterface
    where TContract : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupActionOperation_TContract_.TContract'></a>

`TContract`

The the service contract to which belong operation that is being setup.

Derived  
&#8627; [ISetupOperation&lt;TContract&gt;](ISetupOperation_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupOperation<TContract>')

Implements [IFluentInterface](IFluentInterface.md 'Be.Stateless.BizTalk.IFluentInterface')

| Methods | |
| :--- | :--- |
| [Setup(Expression&lt;Action&lt;TContract&gt;&gt;)](ISetupActionOperation_TContract_.Setup(Expression_Action_TContract__).md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupActionOperation<TContract>.Setup(System.Linq.Expressions.Expression<System.Action<TContract>>)') | Allows to setup what the [IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService') or [ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse') soap stub has to perform upon either the invocation of some SOAP action, that is service contract operation, that produces no result. |
