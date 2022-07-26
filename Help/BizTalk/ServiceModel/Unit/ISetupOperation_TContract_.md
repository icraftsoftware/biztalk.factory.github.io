#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language')

## ISetupOperation<TContract> Interface

Allows to setup what the [IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService') or [ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse') soap stub has to perform upon
the invocation of some SOAP action, that is a service contract's operation.

```csharp
public interface ISetupOperation<TContract> :
Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation<TContract>,
Be.Stateless.BizTalk.IFluentInterface,
Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupActionOperation<TContract>,
Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupOperation
    where TContract : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupOperation_TContract_.TContract'></a>

`TContract`

The the service contract to which belong operation that is being setup.

Implements [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation&lt;](ISetupFunctionOperation_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation<TContract>')[TContract](ISetupOperation_TContract_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupOperation_TContract_.TContract 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupOperation<TContract>.TContract')[&gt;](ISetupFunctionOperation_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation<TContract>'), [IFluentInterface](IFluentInterface.md 'Be.Stateless.BizTalk.IFluentInterface'), [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupActionOperation&lt;](ISetupActionOperation_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupActionOperation<TContract>')[TContract](ISetupOperation_TContract_.md#Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupOperation_TContract_.TContract 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupOperation<TContract>.TContract')[&gt;](ISetupActionOperation_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupActionOperation<TContract>'), [ISetupOperation](ISetupOperation.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupOperation')