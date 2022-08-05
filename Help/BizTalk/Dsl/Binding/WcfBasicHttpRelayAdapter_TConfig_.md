#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## WcfBasicHttpRelayAdapter<TConfig> Class

```csharp
public abstract class WcfBasicHttpRelayAdapter<TConfig> : Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<System.ServiceModel.EndpointAddress, Microsoft.ServiceBus.Configuration.BasicHttpRelayBindingElement, TConfig>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxReceivedMessageSize,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageEncoding,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOptionalAccessControlService,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigAccessControlService,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOptionalSharedAccessSignature,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSharedAccessSignature,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageSecurity<System.ServiceModel.BasicHttpMessageCredentialType>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigServiceCertificate
    where TConfig : Microsoft.BizTalk.Adapter.Wcf.Config.AdapterConfig, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigAddress, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigBasicHttpBinding, Microsoft.BizTalk.Adapter.ServiceBus.IAdapterConfigBasicHttpRelaySecurity, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigAcsCredentials, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigSasCredentials, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigIdentity, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOutboundMessageMarshalling, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigServiceCertificate, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter_TConfig_.TConfig'></a>

`TConfig`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase&lt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.EndpointAddress](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.EndpointAddress 'System.ServiceModel.EndpointAddress')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.ServiceBus.Configuration.BasicHttpRelayBindingElement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.Configuration.BasicHttpRelayBindingElement 'Microsoft.ServiceBus.Configuration.BasicHttpRelayBindingElement')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TConfig](WcfBasicHttpRelayAdapter_TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter_TConfig_.TConfig 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.TConfig')[&gt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase&lt;](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.EndpointAddress](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.EndpointAddress 'System.ServiceModel.EndpointAddress')[,](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.ServiceBus.Configuration.BasicHttpRelayBindingElement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.Configuration.BasicHttpRelayBindingElement 'Microsoft.ServiceBus.Configuration.BasicHttpRelayBindingElement')[,](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')[TConfig](WcfBasicHttpRelayAdapter_TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter_TConfig_.TConfig 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.TConfig')[&gt;](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase&lt;](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.EndpointAddress](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.EndpointAddress 'System.ServiceModel.EndpointAddress')[,](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.ServiceBus.Configuration.BasicHttpRelayBindingElement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.Configuration.BasicHttpRelayBindingElement 'Microsoft.ServiceBus.Configuration.BasicHttpRelayBindingElement')[,](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>')[TConfig](WcfBasicHttpRelayAdapter_TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter_TConfig_.TConfig 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.TConfig')[&gt;](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>') &#129106; WcfBasicHttpRelayAdapter<TConfig>

Derived  
&#8627; [Inbound](WcfBasicHttpRelayAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter.Inbound')  
&#8627; [Outbound](WcfBasicHttpRelayAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter.Outbound')

Implements [IAdapterConfigMaxReceivedMessageSize](IAdapterConfigMaxReceivedMessageSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxReceivedMessageSize'), [IAdapterConfigMessageEncoding](IAdapterConfigMessageEncoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageEncoding'), [IAdapterConfigOptionalAccessControlService](IAdapterConfigOptionalAccessControlService.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOptionalAccessControlService'), [IAdapterConfigAccessControlService](IAdapterConfigAccessControlService.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigAccessControlService'), [IAdapterConfigOptionalSharedAccessSignature](IAdapterConfigOptionalSharedAccessSignature.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOptionalSharedAccessSignature'), [IAdapterConfigSharedAccessSignature](IAdapterConfigSharedAccessSignature.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSharedAccessSignature'), [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode&lt;](IAdapterConfigSecurityMode_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<T>')[Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode 'Microsoft.ServiceBus.EndToEndBasicHttpSecurityMode')[&gt;](IAdapterConfigSecurityMode_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<T>'), [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageSecurity&lt;](IAdapterConfigMessageSecurity_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageSecurity<T>')[System.ServiceModel.BasicHttpMessageCredentialType](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpMessageCredentialType 'System.ServiceModel.BasicHttpMessageCredentialType')[&gt;](IAdapterConfigMessageSecurity_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageSecurity<T>'), [IAdapterConfigServiceCertificate](IAdapterConfigServiceCertificate.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigServiceCertificate')

| Properties | |
| :--- | :--- |
| [AlgorithmSuite](WcfBasicHttpRelayAdapter_TConfig_.AlgorithmSuite.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.AlgorithmSuite') | Specify the message encryption and key-wrap algorithms. These algorithms map to those specified in the Security Policy Language (WS-SecurityPolicy) specification. |
| [IssuerName](WcfBasicHttpRelayAdapter_TConfig_.IssuerName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.IssuerName') | |
| [IssuerSecret](WcfBasicHttpRelayAdapter_TConfig_.IssuerSecret.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.IssuerSecret') | |
| [MaxReceivedMessageSize](WcfBasicHttpRelayAdapter_TConfig_.MaxReceivedMessageSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.MaxReceivedMessageSize') | Specify the maximum size, in bytes, for a message including headers, which can be received on the wire. The size of the messages is bounded by the amount of memory allocated for each message. You can use this property to limit exposure to denial of service (DoS) attacks. |
| [MessageClientCredentialType](WcfBasicHttpRelayAdapter_TConfig_.MessageClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.MessageClientCredentialType') | Specify the message-level security options only if you set the Security mode above to Message or TransportWithMessageCredential. |
| [MessageEncoding](WcfBasicHttpRelayAdapter_TConfig_.MessageEncoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.MessageEncoding') | |
| [RelayClientAuthenticationType](WcfBasicHttpRelayAdapter_TConfig_.RelayClientAuthenticationType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.RelayClientAuthenticationType') | Specify the option to authenticate with the Service Bus relay endpoint from where the message is received. |
| [SecurityMode](WcfBasicHttpRelayAdapter_TConfig_.SecurityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.SecurityMode') | Specify the type of security that is used. |
| [ServiceCertificate](WcfBasicHttpRelayAdapter_TConfig_.ServiceCertificate.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.ServiceCertificate') | |
| [SharedAccessKey](WcfBasicHttpRelayAdapter_TConfig_.SharedAccessKey.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.SharedAccessKey') | |
| [SharedAccessKeyName](WcfBasicHttpRelayAdapter_TConfig_.SharedAccessKeyName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.SharedAccessKeyName') | |
| [StsUri](WcfBasicHttpRelayAdapter_TConfig_.StsUri.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.StsUri') | |
| [TextEncoding](WcfBasicHttpRelayAdapter_TConfig_.TextEncoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.TextEncoding') | Specify the character set encoding to be used for emitting messages on the binding when the [MessageEncoding](WcfBasicHttpRelayAdapter_TConfig_.MessageEncoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.MessageEncoding') property is set to [System.ServiceModel.WSMessageEncoding.Text](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.WSMessageEncoding.Text 'System.ServiceModel.WSMessageEncoding.Text'). |
| [UseAcsAuthentication](WcfBasicHttpRelayAdapter_TConfig_.UseAcsAuthentication.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.UseAcsAuthentication') | |
| [UseSasAuthentication](WcfBasicHttpRelayAdapter_TConfig_.UseSasAuthentication.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.UseSasAuthentication') | |