#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWebHttpAdapter](WcfWebHttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter')

## WcfWebHttpAdapter.Inbound Class

Microsoft BizTalk Server uses the WCF-WebHttp adapter to send messages to RESTful services.

```csharp
public class WcfWebHttpAdapter.Inbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<System.Uri, Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpRLConfig>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundDisableLocationOnFailure,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundIncludeExceptionDetailInFaults,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundSuspendRequestMessageOnFailure,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxConcurrentCalls,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigServiceBehavior,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase&lt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[System.Uri](https://docs.microsoft.com/en-us/dotnet/api/System.Uri 'System.Uri')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.Configuration.WebHttpBindingElement](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Configuration.WebHttpBindingElement 'System.ServiceModel.Configuration.WebHttpBindingElement')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpRLConfig')[&gt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase&lt;](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')[System.Uri](https://docs.microsoft.com/en-us/dotnet/api/System.Uri 'System.Uri')[,](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.Configuration.WebHttpBindingElement](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Configuration.WebHttpBindingElement 'System.ServiceModel.Configuration.WebHttpBindingElement')[,](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpRLConfig')[&gt;](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter&lt;](WcfWebHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>')[System.Uri](https://docs.microsoft.com/en-us/dotnet/api/System.Uri 'System.Uri')[,](WcfWebHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.WebHttpRLConfig')[&gt;](WcfWebHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>') &#129106; Inbound

Implements [IInboundAdapter](IInboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation'), [IAdapterConfigInboundDisableLocationOnFailure](IAdapterConfigInboundDisableLocationOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundDisableLocationOnFailure'), [IAdapterConfigInboundIncludeExceptionDetailInFaults](IAdapterConfigInboundIncludeExceptionDetailInFaults.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundIncludeExceptionDetailInFaults'), [IAdapterConfigInboundSuspendRequestMessageOnFailure](IAdapterConfigInboundSuspendRequestMessageOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundSuspendRequestMessageOnFailure'), [IAdapterConfigMaxConcurrentCalls](IAdapterConfigMaxConcurrentCalls.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxConcurrentCalls'), [IAdapterConfigServiceBehavior](IAdapterConfigServiceBehavior.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigServiceBehavior'), [IAdapterConfigSSO](IAdapterConfigSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO')

### Remarks
The WCF-WebHttp send adapter sends HTTP messages to a service from a BizTalk message. The receive location receives
messages from a RESTful service. For GET and DELETE request, the adapter does not use any payload. For POST and PUT
request, the adapter uses the BizTalk message body part to the HTTP content/payload.

### See Also
- [WCF-WebHttp Adapter](https://docs.microsoft.com/en-us/biztalk/core/wcf-webhttp-adapter 'https://docs.microsoft.com/en-us/biztalk/core/wcf-webhttp-adapter')

| Constructors | |
| :--- | :--- |
| [Inbound()](WcfWebHttpAdapter.Inbound.Inbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Inbound.Inbound()') | |
| [Inbound(Action&lt;Inbound&gt;)](WcfWebHttpAdapter.Inbound.Inbound(Action_Inbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Inbound.Inbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Inbound>)') | |

| Properties | |
| :--- | :--- |
| [AddMessageBodyForHttpVerbs](WcfWebHttpAdapter.Inbound.AddMessageBodyForHttpVerbs.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Inbound.AddMessageBodyForHttpVerbs') | Specify whether to add a empty payload message for some incoming HTTP request made for some HTTP verbs. |
| [DisableLocationOnFailure](WcfWebHttpAdapter.Inbound.DisableLocationOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Inbound.DisableLocationOnFailure') | |
| [IncludeExceptionDetailInFaults](WcfWebHttpAdapter.Inbound.IncludeExceptionDetailInFaults.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Inbound.IncludeExceptionDetailInFaults') | |
| [MaxConcurrentCalls](WcfWebHttpAdapter.Inbound.MaxConcurrentCalls.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Inbound.MaxConcurrentCalls') | |
| [ServiceBehaviors](WcfWebHttpAdapter.Inbound.ServiceBehaviors.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Inbound.ServiceBehaviors') | |
| [SuspendRequestMessageOnFailure](WcfWebHttpAdapter.Inbound.SuspendRequestMessageOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Inbound.SuspendRequestMessageOnFailure') | |
| [UseSSO](WcfWebHttpAdapter.Inbound.UseSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Inbound.UseSSO') | Specify whether to use Enterprise Single Sign-On (SSO) to retrieve client credentials to issue an SSO ticket. |

| Methods | |
| :--- | :--- |
| [Save(IPropertyBag)](WcfWebHttpAdapter.Inbound.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Inbound.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | |
