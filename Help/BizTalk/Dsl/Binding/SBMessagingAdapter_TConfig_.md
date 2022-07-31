#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## SBMessagingAdapter<TConfig> Class

```csharp
public abstract class SBMessagingAdapter<TConfig> : Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigAddress<System.Uri>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOptionalAccessControlService,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigAccessControlService,
Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigSasCredentials
    where TConfig : Microsoft.BizTalk.Adapter.Wcf.Config.AdapterConfig, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigAddress, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigTimeouts, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigAcsCredentials, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigSasCredentials, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter_TConfig_.TConfig'></a>

`TConfig`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; SBMessagingAdapter<TConfig>

Derived  
&#8627; [Inbound](SBMessagingAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Inbound')  
&#8627; [Outbound](SBMessagingAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound')

Implements [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigAddress&lt;](IAdapterConfigAddress_TAddress_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigAddress<TAddress>')[System.Uri](https://docs.microsoft.com/en-us/dotnet/api/System.Uri 'System.Uri')[&gt;](IAdapterConfigAddress_TAddress_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigAddress<TAddress>'), [IAdapterConfigOptionalAccessControlService](IAdapterConfigOptionalAccessControlService.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOptionalAccessControlService'), [IAdapterConfigAccessControlService](IAdapterConfigAccessControlService.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigAccessControlService'), [Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigSasCredentials](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigSasCredentials 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigSasCredentials')

| Properties | |
| :--- | :--- |
| [AdapterConfig](SBMessagingAdapter_TConfig_.AdapterConfig.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>.AdapterConfig') | |
| [Address](SBMessagingAdapter_TConfig_.Address.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>.Address') | Specify the URL where the Service Bus queue is deployed. |
| [CloseTimeout](SBMessagingAdapter_TConfig_.CloseTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>.CloseTimeout') | Specifies a timespan value that indicates the time for a channel close operation to complete. |
| [IssuerName](SBMessagingAdapter_TConfig_.IssuerName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>.IssuerName') | |
| [IssuerSecret](SBMessagingAdapter_TConfig_.IssuerSecret.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>.IssuerSecret') | |
| [OpenTimeout](SBMessagingAdapter_TConfig_.OpenTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>.OpenTimeout') | Specifies a timespan value that indicates the time for a channel open operation to complete. |
| [SharedAccessKey](SBMessagingAdapter_TConfig_.SharedAccessKey.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>.SharedAccessKey') | Specify the SAS key value. |
| [SharedAccessKeyName](SBMessagingAdapter_TConfig_.SharedAccessKeyName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>.SharedAccessKeyName') | Specify the SAS key name. |
| [StsUri](SBMessagingAdapter_TConfig_.StsUri.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>.StsUri') | |
| [UseAcsAuthentication](SBMessagingAdapter_TConfig_.UseAcsAuthentication.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>.UseAcsAuthentication') | |
| [UseSasAuthentication](SBMessagingAdapter_TConfig_.UseSasAuthentication.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>.UseSasAuthentication') | Whether to use Shared Access Signature for authentication. |

| Methods | |
| :--- | :--- |
| [GetAddress()](SBMessagingAdapter_TConfig_.GetAddress().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>.GetAddress()') | |
| [Save(IPropertyBag)](SBMessagingAdapter_TConfig_.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | |
| [Validate()](SBMessagingAdapter_TConfig_.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>.Validate()') | |
