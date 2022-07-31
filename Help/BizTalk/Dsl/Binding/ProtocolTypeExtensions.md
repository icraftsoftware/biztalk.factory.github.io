#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions](Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions')

## ProtocolTypeExtensions Class

Convenient methods to determine an adapter's capabilities as described by its [Microsoft.BizTalk.Deployment.Binding.ProtocolType.Capabilities](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Deployment.Binding.ProtocolType.Capabilities 'Microsoft.BizTalk.Deployment.Binding.ProtocolType.Capabilities')
bitmask value.

```csharp
public static class ProtocolTypeExtensions
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ProtocolTypeExtensions

| Methods | |
| :--- | :--- |
| [RequiresContextInitializationForReceiveHandler(this ProtocolType)](ProtocolTypeExtensions.RequiresContextInitializationForReceiveHandler(thisProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions.ProtocolTypeExtensions.RequiresContextInitializationForReceiveHandler(this Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | Indicates that the adapter uses the Adapter Framework user interface for receive handler configuration. |
| [RequiresContextInitializationForReceiveLocation(this ProtocolType)](ProtocolTypeExtensions.RequiresContextInitializationForReceiveLocation(thisProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions.ProtocolTypeExtensions.RequiresContextInitializationForReceiveLocation(this Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | Indicates that the adapter uses the Adapter Framework user interface for receive location configuration. |
| [RequiresContextInitializationForSendPort(this ProtocolType)](ProtocolTypeExtensions.RequiresContextInitializationForSendPort(thisProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions.ProtocolTypeExtensions.RequiresContextInitializationForSendPort(this Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | Indicates that the adapter uses the Adapter Framework user interface for send port configuration. |
| [RequiresContextInitializationForTransmitHandler(this ProtocolType)](ProtocolTypeExtensions.RequiresContextInitializationForTransmitHandler(thisProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions.ProtocolTypeExtensions.RequiresContextInitializationForTransmitHandler(this Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | Indicates that the adapter uses the Adapter Framework user interface for send handler configuration. |
| [RequiresInProcessHostForReceiveHandler(this ProtocolType)](ProtocolTypeExtensions.RequiresInProcessHostForReceiveHandler(thisProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions.ProtocolTypeExtensions.RequiresInProcessHostForReceiveHandler(this Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | Adapter's receive handler of adapter is hosted in-process.. |
| [RequiresIsolatedHostForReceiveHandler(this ProtocolType)](ProtocolTypeExtensions.RequiresIsolatedHostForReceiveHandler(thisProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions.ProtocolTypeExtensions.RequiresIsolatedHostForReceiveHandler(this Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | Adapter's receive handler of adapter requires an isolated host. |
| [Support32BitOnly(this ProtocolType)](ProtocolTypeExtensions.Support32BitOnly(thisProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions.ProtocolTypeExtensions.Support32BitOnly(this Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | Indicates that the adapter supports running only in 32-bit hosts. |
| [SupportsOrderedDelivery(this ProtocolType)](ProtocolTypeExtensions.SupportsOrderedDelivery(thisProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions.ProtocolTypeExtensions.SupportsOrderedDelivery(this Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | Indicates that the adapter supports ordered delivery of messages. |
| [SupportsReceive(this ProtocolType)](ProtocolTypeExtensions.SupportsReceive(thisProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions.ProtocolTypeExtensions.SupportsReceive(this Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | Adapter supports receive operations. |
| [SupportsRequestResponse(this ProtocolType)](ProtocolTypeExtensions.SupportsRequestResponse(thisProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions.ProtocolTypeExtensions.SupportsRequestResponse(this Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | Adapter supports request-response operations. |
| [SupportsSolicitResponse(this ProtocolType)](ProtocolTypeExtensions.SupportsSolicitResponse(thisProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions.ProtocolTypeExtensions.SupportsSolicitResponse(this Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | Adapter supports solicit-response operations. |
| [SupportsTransmit(this ProtocolType)](ProtocolTypeExtensions.SupportsTransmit(thisProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions.ProtocolTypeExtensions.SupportsTransmit(this Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | Adapter supports send operations. |
| [TransmitAdapterStartsOnServiceStart(this ProtocolType)](ProtocolTypeExtensions.TransmitAdapterStartsOnServiceStart(thisProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Extensions.ProtocolTypeExtensions.TransmitAdapterStartsOnServiceStart(this Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | Send adapter starts when the service starts instead of when it sends the first message. |
