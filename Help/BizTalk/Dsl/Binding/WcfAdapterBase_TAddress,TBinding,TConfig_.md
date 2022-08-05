#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## WcfAdapterBase<TAddress,TBinding,TConfig> Class

Binding DSL base class for all WCF-based BizTalk Server Adapters.

```csharp
public abstract class WcfAdapterBase<TAddress,TBinding,TConfig> : Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigAddress<TAddress>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigBinding<TBinding>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigIdentity
    where TBinding : System.ServiceModel.Configuration.StandardBindingElement, new()
    where TConfig : Microsoft.BizTalk.Adapter.Wcf.Config.AdapterConfig, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigAddress, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigIdentity, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase_TAddress,TBinding,TConfig_.TAddress'></a>

`TAddress`

The address configuration type to which the actual adapter will be connected to. It typically is either [System.ServiceModel.EndpointAddress](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.EndpointAddress 'System.ServiceModel.EndpointAddress') or derived from [Microsoft.ServiceModel.Channels.Common.ConnectionUri](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceModel.Channels.Common.ConnectionUri 'Microsoft.ServiceModel.Channels.Common.ConnectionUri').

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase_TAddress,TBinding,TConfig_.TBinding'></a>

`TBinding`

The [System.ServiceModel.Configuration.StandardBindingElement](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Configuration.StandardBindingElement 'System.ServiceModel.Configuration.StandardBindingElement')-derived class that matches the adapter to be configured.

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase_TAddress,TBinding,TConfig_.TConfig'></a>

`TConfig`

The [AdapterConfig](WcfAdapterBase_TAddress,TBinding,TConfig_.AdapterConfig.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>.AdapterConfig')-derived class that matches the adapter to be configured.

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; WcfAdapterBase<TAddress,TBinding,TConfig>

Derived  
&#8627; [WcfBindingCentricAdapterBase&lt;TAddress,TBinding,TConfig&gt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')  
&#8627; [WcfOneWayAdapterBase&lt;TAddress,TBinding,TConfig&gt;](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')

Implements [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigAddress&lt;](IAdapterConfigAddress_TAddress_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigAddress<TAddress>')[TAddress](WcfAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase_TAddress,TBinding,TConfig_.TAddress 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>.TAddress')[&gt;](IAdapterConfigAddress_TAddress_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigAddress<TAddress>'), [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigBinding&lt;](IAdapterConfigBinding_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigBinding<T>')[TBinding](WcfAdapterBase_TAddress,TBinding,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase_TAddress,TBinding,TConfig_.TBinding 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>.TBinding')[&gt;](IAdapterConfigBinding_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigBinding<T>'), [IAdapterConfigIdentity](IAdapterConfigIdentity.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigIdentity')

### See Also
- [WCF Adapters](https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters 'https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters')
- [What Are the WCF Adapters?](https://docs.microsoft.com/en-us/biztalk/core/what-are-the-wcf-adapters 'https://docs.microsoft.com/en-us/biztalk/core/what-are-the-wcf-adapters')
- [WCF Adapters Property Schema and Properties](https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters-property-schema-and-properties 'https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters-property-schema-and-properties')

| Constructors | |
| :--- | :--- |
| [WcfAdapterBase(ProtocolType)](WcfAdapterBase_TAddress,TBinding,TConfig_.WcfAdapterBase(ProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>.WcfAdapterBase(Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | |

| Properties | |
| :--- | :--- |
| [AdapterConfig](WcfAdapterBase_TAddress,TBinding,TConfig_.AdapterConfig.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>.AdapterConfig') | |
| [Address](WcfAdapterBase_TAddress,TBinding,TConfig_.Address.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>.Address') | |
| [BindingElement](WcfAdapterBase_TAddress,TBinding,TConfig_.BindingElement.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>.BindingElement') | |
| [Identity](WcfAdapterBase_TAddress,TBinding,TConfig_.Identity.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>.Identity') | Specify the identity of the service that this receive location provides. |

| Methods | |
| :--- | :--- |
| [GetAddress()](WcfAdapterBase_TAddress,TBinding,TConfig_.GetAddress().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>.GetAddress()') | |
| [Save(IPropertyBag)](WcfAdapterBase_TAddress,TBinding,TConfig_.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | |
| [Validate()](WcfAdapterBase_TAddress,TBinding,TConfig_.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>.Validate()') | |

| Explicit Interface Implementations | |
| :--- | :--- |
| [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigBinding&lt;TBinding&gt;.Binding](WcfAdapterBase_TAddress,TBinding,TConfig_.Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigBinding_TBinding_.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>.Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigBinding<TBinding>.Binding') | |
