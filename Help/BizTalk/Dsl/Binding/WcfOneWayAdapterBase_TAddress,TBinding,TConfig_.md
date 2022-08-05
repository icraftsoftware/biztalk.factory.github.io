#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## WcfOneWayAdapterBase<TAddress,TBinding,TConfig> Class

```csharp
public abstract class WcfOneWayAdapterBase<TAddress,TBinding,TConfig> : Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress, TBinding, TConfig>,
Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts
    where TBinding : System.ServiceModel.Configuration.StandardBindingElement, new()
    where TConfig : Microsoft.BizTalk.Adapter.Wcf.Config.AdapterConfig, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigAddress, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigIdentity, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.TAddress'></a>

`TAddress`

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.TBinding'></a>

`TBinding`

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.TConfig'></a>

`TConfig`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase&lt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TAddress](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.TAddress 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>.TAddress')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TBinding](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>.TBinding')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TConfig](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.TConfig 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>.TConfig')[&gt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>') &#129106; WcfOneWayAdapterBase<TAddress,TBinding,TConfig>

Derived  
&#8627; [WcfNetMsmqAdapter&lt;TConfig&gt;](WcfNetMsmqAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>')  
&#8627; [WcfTwoWayAdapterBase&lt;TAddress,TBinding,TConfig&gt;](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>')  
&#8627; [WcfWebHttpAdapter&lt;TAddress,TConfig&gt;](WcfWebHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>')

Implements [Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts')

| Constructors | |
| :--- | :--- |
| [WcfOneWayAdapterBase(ProtocolType)](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.WcfOneWayAdapterBase(ProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>.WcfOneWayAdapterBase(Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | |

| Properties | |
| :--- | :--- |
| [CloseTimeout](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.CloseTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>.CloseTimeout') | Gets or sets the interval of time after which the close method, invoked by a communication object, times out. |
| [OpenTimeout](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.OpenTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>.OpenTimeout') | Gets or sets the interval of time after which the open method, invoked by a communication object, times out. |
| [SendTimeout](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.SendTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>.SendTimeout') | Gets or sets the interval of time after which the send method, invoked by a communication object, times out. |
