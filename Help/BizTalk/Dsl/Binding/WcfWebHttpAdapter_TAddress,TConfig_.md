#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## WcfWebHttpAdapter<TAddress,TConfig> Class

```csharp
public abstract class WcfWebHttpAdapter<TAddress,TConfig> : Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress, System.ServiceModel.Configuration.WebHttpBindingElement, TConfig>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigEndpointBehavior,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxReceivedMessageSize,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigServiceCertificate,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigTransportSecurity<System.ServiceModel.HttpClientCredentialType>
    where TConfig : Microsoft.BizTalk.Adapter.Wcf.Config.AdapterConfig, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigAddress, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigEndpointBehavior, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigIdentity, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOutboundHttpProperty, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigRequestHttpProperty, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigServiceCertificate, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigVariablePropertyMapping, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigWebHttpBinding, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigWebHttpSecurity, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter_TAddress,TConfig_.TAddress'></a>

`TAddress`

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter_TAddress,TConfig_.TConfig'></a>

`TConfig`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase&lt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TAddress](WcfWebHttpAdapter_TAddress,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter_TAddress,TConfig_.TAddress 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.TAddress')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.Configuration.WebHttpBindingElement](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Configuration.WebHttpBindingElement 'System.ServiceModel.Configuration.WebHttpBindingElement')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TConfig](WcfWebHttpAdapter_TAddress,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter_TAddress,TConfig_.TConfig 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.TConfig')[&gt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase&lt;](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')[TAddress](WcfWebHttpAdapter_TAddress,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter_TAddress,TConfig_.TAddress 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.TAddress')[,](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.Configuration.WebHttpBindingElement](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Configuration.WebHttpBindingElement 'System.ServiceModel.Configuration.WebHttpBindingElement')[,](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')[TConfig](WcfWebHttpAdapter_TAddress,TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter_TAddress,TConfig_.TConfig 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.TConfig')[&gt;](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>') &#129106; WcfWebHttpAdapter<TAddress,TConfig>

Derived  
&#8627; [Inbound](WcfWebHttpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Inbound')  
&#8627; [Outbound](WcfWebHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound')

Implements [IAdapterConfigEndpointBehavior](IAdapterConfigEndpointBehavior.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigEndpointBehavior'), [IAdapterConfigMaxReceivedMessageSize](IAdapterConfigMaxReceivedMessageSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxReceivedMessageSize'), [IAdapterConfigServiceCertificate](IAdapterConfigServiceCertificate.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigServiceCertificate'), [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode&lt;](IAdapterConfigSecurityMode_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<T>')[Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode 'Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpSecurityMode')[&gt;](IAdapterConfigSecurityMode_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<T>'), [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigTransportSecurity&lt;](IAdapterConfigTransportSecurity_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigTransportSecurity<T>')[System.ServiceModel.HttpClientCredentialType](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType 'System.ServiceModel.HttpClientCredentialType')[&gt;](IAdapterConfigTransportSecurity_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigTransportSecurity<T>')

| Properties | |
| :--- | :--- |
| [EndpointBehaviors](WcfWebHttpAdapter_TAddress,TConfig_.EndpointBehaviors.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.EndpointBehaviors') | |
| [HttpHeaders](WcfWebHttpAdapter_TAddress,TConfig_.HttpHeaders.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.HttpHeaders') | Specifies the HTTP headers that are stamped on the response message. |
| [HttpUrlMapping](WcfWebHttpAdapter_TAddress,TConfig_.HttpUrlMapping.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.HttpUrlMapping') | BTS Operation Mapping allows users to map incoming HTTP requests to BTS Operation in the message context, based on the incoming HTTP Method and the URL sub-path. |
| [MaxReceivedMessageSize](WcfWebHttpAdapter_TAddress,TConfig_.MaxReceivedMessageSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.MaxReceivedMessageSize') | Specify the maximum size, in bytes, for a message including headers, which can be received on the wire. The size of the messages is bounded by the amount of memory allocated for each message. You can use this property to limit exposure to denial of service (DoS) attacks. |
| [SecurityMode](WcfWebHttpAdapter_TAddress,TConfig_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.SecurityMode') | Specify the type of security that is used. |
| [ServiceCertificate](WcfWebHttpAdapter_TAddress,TConfig_.ServiceCertificate.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.ServiceCertificate') | |
| [TransportClientCredentialType](WcfWebHttpAdapter_TAddress,TConfig_.TransportClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.TransportClientCredentialType') | Specify the type of credential to be used when performing the client authentication. |
| [VariableMapping](WcfWebHttpAdapter_TAddress,TConfig_.VariableMapping.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.VariableMapping') | Allows to specify what the variable maps to at runtime if variables have been declared in the HTTP Method URL Mappings. |

| Methods | |
| :--- | :--- |
| [Save(IPropertyBag)](WcfWebHttpAdapter_TAddress,TConfig_.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | |
