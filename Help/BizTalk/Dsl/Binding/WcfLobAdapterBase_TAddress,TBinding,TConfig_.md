#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## WcfLobAdapterBase<TAddress,TBinding,TConfig> Class

```csharp
public abstract class WcfLobAdapterBase<TAddress,TBinding,TConfig> : Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress, TBinding, TConfig>
    where TBinding : System.ServiceModel.Configuration.StandardBindingElement, new()
    where TConfig : Microsoft.BizTalk.Adapter.Wcf.Config.AdapterConfig, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigAddress, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigIdentity, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigBinding, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigEndpointBehavior, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOutboundMessageMarshalling, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase_TAddress,TBinding,TConfig_.TAddress'></a>

`TAddress`

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase_TAddress,TBinding,TConfig_.TBinding'></a>

`TBinding`

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase_TAddress,TBinding,TConfig_.TConfig'></a>

`TConfig`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase&lt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TAddress](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase_TAddress,TBinding,TConfig_.TAddress 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>.TAddress')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TBinding](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase_TAddress,TBinding,TConfig_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>.TBinding')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TConfig](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase_TAddress,TBinding,TConfig_.TConfig 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>.TConfig')[&gt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase&lt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[TAddress](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase_TAddress,TBinding,TConfig_.TAddress 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>.TAddress')[,](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[TBinding](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase_TAddress,TBinding,TConfig_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>.TBinding')[,](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[TConfig](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase_TAddress,TBinding,TConfig_.TConfig 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>.TConfig')[&gt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>') &#129106; WcfLobAdapterBase<TAddress,TBinding,TConfig>

Derived  
&#8627; [WcfOracleAdapter&lt;TConfig&gt;](WcfOracleAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>')  
&#8627; [WcfSapAdapter&lt;TConfig&gt;](WcfSapAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter<TConfig>')  
&#8627; [WcfSqlAdapter&lt;TConfig&gt;](WcfSqlAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter<TConfig>')

| Constructors | |
| :--- | :--- |
| [WcfLobAdapterBase(ProtocolType)](WcfLobAdapterBase_TAddress,TBinding,TConfig_.WcfLobAdapterBase(ProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>.WcfLobAdapterBase(Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | |

| Properties | |
| :--- | :--- |
| [ReceiveTimeout](WcfLobAdapterBase_TAddress,TBinding,TConfig_.ReceiveTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>.ReceiveTimeout') | Gets or sets the interval of time after which the receive method, invoked by a communication object, times out. |
