#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## WcfCustomAdapterBase<TAddress,TBinding,TConfig> Class

```csharp
public abstract class WcfCustomAdapterBase<TAddress,TBinding,TConfig> : Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress, TBinding, TConfig>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigBinding<TBinding>
    where TBinding : System.ServiceModel.Configuration.StandardBindingElement, new()
    where TConfig : Microsoft.BizTalk.Adapter.Wcf.Config.AdapterConfig, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigAddress, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigIdentity, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigBinding, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigEndpointBehavior, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOutboundMessageMarshalling, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase_TAddress,TBinding,TConfig_.TAddress'></a>

`TAddress`

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase_TAddress,TBinding,TConfig_.TBinding'></a>

`TBinding`

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase_TAddress,TBinding,TConfig_.TConfig'></a>

`TConfig`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase&lt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TAddress](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase_TAddress,TBinding,TConfig_.TAddress 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>.TAddress')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TBinding](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase_TAddress,TBinding,TConfig_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>.TBinding')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TConfig](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase_TAddress,TBinding,TConfig_.TConfig 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>.TConfig')[&gt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase&lt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[TAddress](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase_TAddress,TBinding,TConfig_.TAddress 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>.TAddress')[,](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[TBinding](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase_TAddress,TBinding,TConfig_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>.TBinding')[,](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[TConfig](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase_TAddress,TBinding,TConfig_.TConfig 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>.TConfig')[&gt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>') &#129106; WcfCustomAdapterBase<TAddress,TBinding,TConfig>

Derived  
&#8627; [WcfCustomAdapter&lt;TBinding,TConfig&gt;](WcfCustomAdapter_TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter<TBinding,TConfig>')  
&#8627; [WcfCustomIsolatedAdapter&lt;TBinding,TConfig&gt;](WcfCustomIsolatedAdapter_TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter<TBinding,TConfig>')

Implements [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigBinding&lt;](IAdapterConfigBinding_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigBinding<T>')[TBinding](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase_TAddress,TBinding,TConfig_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>.TBinding')[&gt;](IAdapterConfigBinding_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigBinding<T>')

| Constructors | |
| :--- | :--- |
| [WcfCustomAdapterBase(ProtocolType)](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.WcfCustomAdapterBase(ProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>.WcfCustomAdapterBase(Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | |

| Properties | |
| :--- | :--- |
| [Binding](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>.Binding') | |

| Methods | |
| :--- | :--- |
| [Validate()](WcfCustomAdapterBase_TAddress,TBinding,TConfig_.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapterBase<TAddress,TBinding,TConfig>.Validate()') | |
