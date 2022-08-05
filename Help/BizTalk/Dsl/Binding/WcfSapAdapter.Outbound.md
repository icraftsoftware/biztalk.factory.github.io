#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSapAdapter](WcfSapAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter')

## WcfSapAdapter.Outbound Class

The Microsoft BizTalk Adapter for mySAP Business Suite exposes the SAP system as a WCF service. Adapter
clients can perform operations on the SAP system by exchanging SOAP messages with the adapter. The adapter
consumes the WCF message and makes appropriate calls to the SAP system to perform the operation. The adapter
returns the response from the SAP system back to the client in the form of SOAP messages.

```csharp
public class WcfSapAdapter.Outbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter<Microsoft.BizTalk.Adapter.Wcf.Config.CustomTLConfig>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IOutboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundAction,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundCredentials,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundPropagateFaultMessage,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundTransactionIsolation
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase&lt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.Adapters.SAP.SAPConnectionUri](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.SAP.SAPConnectionUri 'Microsoft.Adapters.SAP.SAPConnectionUri')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.Adapters.SAP.SAPAdapterBindingConfigurationElement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.SAP.SAPAdapterBindingConfigurationElement 'Microsoft.Adapters.SAP.SAPAdapterBindingConfigurationElement')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.CustomTLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CustomTLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.CustomTLConfig')[&gt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase&lt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.Adapters.SAP.SAPConnectionUri](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.SAP.SAPConnectionUri 'Microsoft.Adapters.SAP.SAPConnectionUri')[,](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.Adapters.SAP.SAPAdapterBindingConfigurationElement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.SAP.SAPAdapterBindingConfigurationElement 'Microsoft.Adapters.SAP.SAPAdapterBindingConfigurationElement')[,](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.CustomTLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CustomTLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.CustomTLConfig')[&gt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase&lt;](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.Adapters.SAP.SAPConnectionUri](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.SAP.SAPConnectionUri 'Microsoft.Adapters.SAP.SAPConnectionUri')[,](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.Adapters.SAP.SAPAdapterBindingConfigurationElement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.SAP.SAPAdapterBindingConfigurationElement 'Microsoft.Adapters.SAP.SAPAdapterBindingConfigurationElement')[,](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.CustomTLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CustomTLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.CustomTLConfig')[&gt;](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter&lt;](WcfSapAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter<TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.CustomTLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CustomTLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.CustomTLConfig')[&gt;](WcfSapAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter<TConfig>') &#129106; Outbound

Implements [IOutboundAdapter](IOutboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IOutboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation'), [IAdapterConfigOutboundAction](IAdapterConfigOutboundAction.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundAction'), [IAdapterConfigOutboundCredentials](IAdapterConfigOutboundCredentials.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundCredentials'), [IAdapterConfigSSO](IAdapterConfigSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO'), [IAdapterConfigOutboundPropagateFaultMessage](IAdapterConfigOutboundPropagateFaultMessage.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundPropagateFaultMessage'), [IAdapterConfigOutboundTransactionIsolation](IAdapterConfigOutboundTransactionIsolation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundTransactionIsolation')

### See Also
- [Overview of BizTalk Adapter for mySAP Business Suite](https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-sap/overview-of-the-sap-adapter 'https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-sap/overview-of-the-sap-adapter')
- [Read about BizTalk Adapter for mySAP Business Suite binding properties](https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-sap/read-about-biztalk-adapter-for-mysap-business-suite-binding-properties 'https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-sap/read-about-biztalk-adapter-for-mysap-business-suite-binding-properties')
- [Understanding BizTalk Adapter for mySAP Business Suite](https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-sap/understand-biztalk-adapter-for-mysap-business-suite 'https://docs.microsoft.com/en-us/biztalk/adapters-and-accelerators/adapter-sap/understand-biztalk-adapter-for-mysap-business-suite')
- [WCF Adapters Property Schema and Properties](https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters-property-schema-and-properties 'https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters-property-schema-and-properties')

| Constructors | |
| :--- | :--- |
| [Outbound()](WcfSapAdapter.Outbound.Outbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound.Outbound()') | |
| [Outbound(Action&lt;Outbound&gt;)](WcfSapAdapter.Outbound.Outbound(Action_Outbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound.Outbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound>)') | |

| Properties | |
| :--- | :--- |
| [AffiliateApplicationName](WcfSapAdapter.Outbound.AffiliateApplicationName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound.AffiliateApplicationName') | |
| [AutoConfirmSentIdocs](WcfSapAdapter.Outbound.AutoConfirmSentIdocs.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound.AutoConfirmSentIdocs') | Determines whether the adapter automatically calls RfcConfirmTransID() after sending an IDoc. |
| [ClearRfcContext](WcfSapAdapter.Outbound.ClearRfcContext.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound.ClearRfcContext') | Determines whether the state acquired by the R/3 user context should be reset before returning a connection back to the connection pool. |
| [EnableTransaction](WcfSapAdapter.Outbound.EnableTransaction.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound.EnableTransaction') | |
| [IsolationLevel](WcfSapAdapter.Outbound.IsolationLevel.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound.IsolationLevel') | |
| [Password](WcfSapAdapter.Outbound.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound.Password') | |
| [PropagateFaultMessage](WcfSapAdapter.Outbound.PropagateFaultMessage.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound.PropagateFaultMessage') | |
| [StaticAction](WcfSapAdapter.Outbound.StaticAction.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound.StaticAction') | |
| [UserName](WcfSapAdapter.Outbound.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound.UserName') | |
| [UseSSO](WcfSapAdapter.Outbound.UseSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound.UseSSO') | |