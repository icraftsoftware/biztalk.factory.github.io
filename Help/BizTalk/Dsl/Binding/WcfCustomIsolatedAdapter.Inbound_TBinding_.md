#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfCustomIsolatedAdapter](WcfCustomIsolatedAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter')

## WcfCustomIsolatedAdapter.Inbound<TBinding> Class

The WCF-CustomIsolated adapter is used to enable the use of WCF extensibility components in BizTalk Server with an
isolated host. The adapter enables complete flexibility of the WCF framework. It allows users to select and configure
a WCF binding for the receive location, and to specify the endpoint behaviors and security settings. This adapter can
only be used by transports that are hosted in Internet Information Services (IIS).

```csharp
public class WcfCustomIsolatedAdapter.Inbound<TBinding> : Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter<TBinding, Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig>,
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

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound_TBinding_.TBinding'></a>

`TBinding`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase&lt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[System.Uri](https://docs.microsoft.com/en-us/dotnet/api/System.Uri 'System.Uri')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TBinding](WcfCustomIsolatedAdapter.Inbound_TBinding_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound_TBinding_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.TBinding')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig')[&gt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase&lt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[System.Uri](https://docs.microsoft.com/en-us/dotnet/api/System.Uri 'System.Uri')[,](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[TBinding](WcfCustomIsolatedAdapter.Inbound_TBinding_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound_TBinding_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.TBinding')[,](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig')[&gt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase&lt;](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>')[System.Uri](https://docs.microsoft.com/en-us/dotnet/api/System.Uri 'System.Uri')[,](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>')[TBinding](WcfCustomIsolatedAdapter.Inbound_TBinding_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound_TBinding_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.TBinding')[,](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig')[&gt;](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter&lt;](WcfCustomIsolatedAdapter_TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter<TBinding,TConfig>')[TBinding](WcfCustomIsolatedAdapter.Inbound_TBinding_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound_TBinding_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.TBinding')[,](WcfCustomIsolatedAdapter_TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter<TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.CustomRLConfig')[&gt;](WcfCustomIsolatedAdapter_TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter<TBinding,TConfig>') &#129106; Inbound<TBinding>

Implements [IInboundAdapter](IInboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation'), [IAdapterConfigInboundCredentials](IAdapterConfigInboundCredentials.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials'), [IAdapterConfigInboundDisableLocationOnFailure](IAdapterConfigInboundDisableLocationOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundDisableLocationOnFailure'), [IAdapterConfigInboundIncludeExceptionDetailInFaults](IAdapterConfigInboundIncludeExceptionDetailInFaults.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundIncludeExceptionDetailInFaults'), [IAdapterConfigInboundSuspendRequestMessageOnFailure](IAdapterConfigInboundSuspendRequestMessageOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundSuspendRequestMessageOnFailure'), [Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOrdering](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOrdering 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOrdering'), [IAdapterConfigServiceBehavior](IAdapterConfigServiceBehavior.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigServiceBehavior')

### Remarks
The WCF-CustomIsolated adapter consists of a receive adapter only. You use the WCF-CustomIsolated receive adapter to
receive WCF service requests through WCF bindings, service behavior, endpoint behavior, security mechanism, and the
source of the inbound message body that you selected and configured for the receive location running in an isolated
host. A receive location that uses the WCF-CustomIsolated receive adapter can be configured as one-way or
request-response (two-way).

### See Also
- [WCF-CustomIsolated Adapter](https://docs.microsoft.com/en-us/biztalk/core/wcf-customisolated-adapter 'https://docs.microsoft.com/en-us/biztalk/core/wcf-customisolated-adapter')
- [What Is the WCF-CustomIsolated Adapter?](https://docs.microsoft.com/en-us/biztalk/core/what-is-the-wcf-customisolated-adapter 'https://docs.microsoft.com/en-us/biztalk/core/what-is-the-wcf-customisolated-adapter')
- [How to Configure a WCF-CustomIsolated Receive Location](https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-a-wcf-customisolated-receive-location 'https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-a-wcf-customisolated-receive-location')
- [WCF Adapters Property Schema and Properties](https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters-property-schema-and-properties 'https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters-property-schema-and-properties')

| Constructors | |
| :--- | :--- |
| [Inbound()](WcfCustomIsolatedAdapter.Inbound_TBinding_.Inbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.Inbound()') | |
| [Inbound(Action&lt;Inbound&lt;TBinding&gt;&gt;)](WcfCustomIsolatedAdapter.Inbound_TBinding_.Inbound(Action_Inbound_TBinding__).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.Inbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>>)') | |

| Properties | |
| :--- | :--- |
| [AffiliateApplicationName](WcfCustomIsolatedAdapter.Inbound_TBinding_.AffiliateApplicationName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.AffiliateApplicationName') | |
| [CredentialType](WcfCustomIsolatedAdapter.Inbound_TBinding_.CredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.CredentialType') | |
| [DisableLocationOnFailure](WcfCustomIsolatedAdapter.Inbound_TBinding_.DisableLocationOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.DisableLocationOnFailure') | |
| [IncludeExceptionDetailInFaults](WcfCustomIsolatedAdapter.Inbound_TBinding_.IncludeExceptionDetailInFaults.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.IncludeExceptionDetailInFaults') | |
| [OrderedProcessing](WcfCustomIsolatedAdapter.Inbound_TBinding_.OrderedProcessing.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.OrderedProcessing') | Specify whether to preserve message order when processing messages received over the NetMsmq binding. |
| [Password](WcfCustomIsolatedAdapter.Inbound_TBinding_.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.Password') | |
| [ReceiveTimeout](WcfCustomIsolatedAdapter.Inbound_TBinding_.ReceiveTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.ReceiveTimeout') | On the service side, initialize the session-idle timeout which controls how long a session can be idle before timing out. |
| [ServiceBehaviors](WcfCustomIsolatedAdapter.Inbound_TBinding_.ServiceBehaviors.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.ServiceBehaviors') | |
| [SuspendRequestMessageOnFailure](WcfCustomIsolatedAdapter.Inbound_TBinding_.SuspendRequestMessageOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.SuspendRequestMessageOnFailure') | |
| [UserName](WcfCustomIsolatedAdapter.Inbound_TBinding_.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.UserName') | |

| Methods | |
| :--- | :--- |
| [Save(IPropertyBag)](WcfCustomIsolatedAdapter.Inbound_TBinding_.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | |
