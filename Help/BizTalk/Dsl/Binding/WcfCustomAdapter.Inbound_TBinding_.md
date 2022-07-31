#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfCustomAdapter](WcfCustomAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter')

## WcfCustomAdapter.Inbound<TBinding> Class

The WCF-Custom adapter is used to enable the use of WCF extensibility components in BizTalk Server. The adapter
enables complete flexibility of the WCF framework. It allows users to select and configure a WCF binding for the
receive location and send port. It also allows users to set the endpoint behaviors and security settings.

```csharp
public class WcfCustomAdapter.Inbound<TBinding> : Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter<TBinding, Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundDisableLocationOnFailure,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundIncludeExceptionDetailInFaults,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundSuspendRequestMessageOnFailure,
Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOrdering,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigServiceBehavior
    where TBinding : System.ServiceModel.Configuration.StandardBindingElement, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound_TBinding_.TBinding'></a>

`TBinding`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase&lt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.EndpointAddress](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.EndpointAddress 'System.ServiceModel.EndpointAddress')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TBinding](WcfCustomAdapter.Inbound_TBinding_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound_TBinding_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.TBinding')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig')[&gt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase&lt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.EndpointAddress](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.EndpointAddress 'System.ServiceModel.EndpointAddress')[,](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[TBinding](WcfCustomAdapter.Inbound_TBinding_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound_TBinding_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.TBinding')[,](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig')[&gt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase&lt;](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.EndpointAddress](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.EndpointAddress 'System.ServiceModel.EndpointAddress')[,](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>')[TBinding](WcfCustomAdapter.Inbound_TBinding_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound_TBinding_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.TBinding')[,](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig')[&gt;](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter&lt;](WcfCustomAdapter_TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter<TBinding,TConfig>')[TBinding](WcfCustomAdapter.Inbound_TBinding_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound_TBinding_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.TBinding')[,](WcfCustomAdapter_TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter<TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig')[&gt;](WcfCustomAdapter_TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter<TBinding,TConfig>') &#129106; Inbound<TBinding>

Implements [IInboundAdapter](IInboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation'), [IAdapterConfigInboundCredentials](IAdapterConfigInboundCredentials.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials'), [IAdapterConfigInboundDisableLocationOnFailure](IAdapterConfigInboundDisableLocationOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundDisableLocationOnFailure'), [IAdapterConfigInboundIncludeExceptionDetailInFaults](IAdapterConfigInboundIncludeExceptionDetailInFaults.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundIncludeExceptionDetailInFaults'), [IAdapterConfigInboundSuspendRequestMessageOnFailure](IAdapterConfigInboundSuspendRequestMessageOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundSuspendRequestMessageOnFailure'), [Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOrdering](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOrdering 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOrdering'), [IAdapterConfigServiceBehavior](IAdapterConfigServiceBehavior.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigServiceBehavior')

### Remarks
You use the WCF-Custom receive adapter to receive WCF service requests through the bindings, service behavior,
endpoint behavior, security mechanism, and the source of the inbound message body that you selected and configured in
the transport properties dialog in the receive location. A receive location that uses the WCF-Custom receive adapter
can be configured as one-way or request-response (two-way).

### See Also
- [What Is the WCF-Custom Adapter?](https://docs.microsoft.com/en-us/biztalk/core/what-is-the-wcf-custom-adapter 'https://docs.microsoft.com/en-us/biztalk/core/what-is-the-wcf-custom-adapter')
- [How to Configure a WCF-Custom Receive Location](https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-a-wcf-custom-receive-location 'https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-a-wcf-custom-receive-location')
- [WCF Adapters Property Schema and Properties](https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters-property-schema-and-properties 'https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters-property-schema-and-properties')

| Constructors | |
| :--- | :--- |
| [Inbound()](WcfCustomAdapter.Inbound_TBinding_.Inbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.Inbound()') | |
| [Inbound(Action&lt;Inbound&lt;TBinding&gt;&gt;)](WcfCustomAdapter.Inbound_TBinding_.Inbound(Action_Inbound_TBinding__).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.Inbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>>)') | |

| Properties | |
| :--- | :--- |
| [AffiliateApplicationName](WcfCustomAdapter.Inbound_TBinding_.AffiliateApplicationName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.AffiliateApplicationName') | |
| [CredentialType](WcfCustomAdapter.Inbound_TBinding_.CredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.CredentialType') | |
| [DisableLocationOnFailure](WcfCustomAdapter.Inbound_TBinding_.DisableLocationOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.DisableLocationOnFailure') | |
| [IncludeExceptionDetailInFaults](WcfCustomAdapter.Inbound_TBinding_.IncludeExceptionDetailInFaults.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.IncludeExceptionDetailInFaults') | |
| [OrderedProcessing](WcfCustomAdapter.Inbound_TBinding_.OrderedProcessing.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.OrderedProcessing') | Specify whether to preserve message order when processing messages received over the NetMsmq binding. |
| [Password](WcfCustomAdapter.Inbound_TBinding_.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.Password') | |
| [ReceiveTimeout](WcfCustomAdapter.Inbound_TBinding_.ReceiveTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.ReceiveTimeout') | On the service side, initialize the session-idle timeout which controls how long a session can be idle before timing out. |
| [ServiceBehaviors](WcfCustomAdapter.Inbound_TBinding_.ServiceBehaviors.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.ServiceBehaviors') | |
| [SuspendRequestMessageOnFailure](WcfCustomAdapter.Inbound_TBinding_.SuspendRequestMessageOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.SuspendRequestMessageOnFailure') | |
| [UserName](WcfCustomAdapter.Inbound_TBinding_.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.UserName') | |

| Methods | |
| :--- | :--- |
| [Save(IPropertyBag)](WcfCustomAdapter.Inbound_TBinding_.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | |
