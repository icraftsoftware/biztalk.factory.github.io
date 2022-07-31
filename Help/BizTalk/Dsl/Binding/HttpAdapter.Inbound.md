#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter')

## HttpAdapter.Inbound Class

You use the HTTP adapter to exchange information between Microsoft BizTalk Server and an application by means of the
HTTP protocol. HTTP is the primary protocol for inter-business message exchange. Applications can send messages to a
server by sending HTTP POST or HTTP GET requests to a specified HTTP URL. The HTTP adapter receives the HTTP requests
and submits them to BizTalk Server for processing. Similarly, BizTalk Server can transmit messages to remote
applications by sending HTTP POST requests to a specified HTTP URL.

```csharp
public class HttpAdapter.Inbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundSuspendRequestMessageOnFailure,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter') &#129106; Inbound

Implements [IInboundAdapter](IInboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation'), [IAdapterConfigInboundSuspendRequestMessageOnFailure](IAdapterConfigInboundSuspendRequestMessageOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundSuspendRequestMessageOnFailure'), [IAdapterConfigSSO](IAdapterConfigSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO')

### Remarks
The HTTP receive adapter is a Microsoft Internet Information Services (IIS) Internet Server Application Programming
Interface (ISAPI) extension that the IIS process hosts, and controls the receive locations that use the HTTP adapter.

### See Also
- [HTTP Adapter](https://docs.microsoft.com/en-us/biztalk/core/http-adapter 'https://docs.microsoft.com/en-us/biztalk/core/http-adapter')
- [Configuring the HTTP Adapter](https://docs.microsoft.com/en-us/biztalk/core/configuring-the-http-adapter 'https://docs.microsoft.com/en-us/biztalk/core/configuring-the-http-adapter')
- [HTTP Receive Adapter](https://docs.microsoft.com/en-us/biztalk/core/http-receive-adapter 'https://docs.microsoft.com/en-us/biztalk/core/http-receive-adapter')
- [How to Configure an HTTP Receive Handler](https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-an-http-receive-handler 'https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-an-http-receive-handler')
- [How to Configure IIS for an HTTP Receive Location](https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-iis-for-an-http-receive-location 'https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-iis-for-an-http-receive-location')
- [How to Configure an HTTP Receive Location](https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-an-http-receive-location 'https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-an-http-receive-location')

| Constructors | |
| :--- | :--- |
| [Inbound()](HttpAdapter.Inbound.Inbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound.Inbound()') | |
| [Inbound(Action&lt;Inbound&gt;)](HttpAdapter.Inbound.Inbound(Action_Inbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound.Inbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound>)') | |

| Properties | |
| :--- | :--- |
| [LoopBack](HttpAdapter.Inbound.LoopBack.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound.LoopBack') | Specifies that the request message received on this location will be routed either to a send port or back to the receive location to be sent as a response. This property is valid only for request-response receive ports. It is ignored for one-way receive ports. |
| [Path](HttpAdapter.Inbound.Path.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound.Path') | Specify the name of the virtual directory where you post the messages received by the HTTP/HTTPS receive location. The virtual directory includes the name of the receive location DLL and an optional query string. |
| [ResponseContentType](HttpAdapter.Inbound.ResponseContentType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound.ResponseContentType') | Content type of the HTTP response messages that the HTTP adapter sends back to clients from this receive location. This property is valid only for request-response receive ports and is ignored for one-way receive ports. |
| [ReturnCorrelationHandle](HttpAdapter.Inbound.ReturnCorrelationHandle.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound.ReturnCorrelationHandle') | Specifies that the correlation token of submitted message that the HTTP adapter sends on HTTP response to the client if the submission is successful. This property is valid only for one-way receive ports and is ignored for request-response receive ports. |
| [SuspendRequestMessageOnFailure](HttpAdapter.Inbound.SuspendRequestMessageOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound.SuspendRequestMessageOnFailure') | Indicate whether or not to suspend HTTP requests that fail inbound processing. |
| [Url](HttpAdapter.Inbound.Url.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound.Url') | Specify the fully qualified URI for this receive location. The value for this property is a combination of the server name and the virtual directory. The BizTalk Messaging Engine exposes this address to external partners. The specified URI should designate the public Web site URL for trading partners to connect to when sending messages to BizTalk Server. |
| [UseSSO](HttpAdapter.Inbound.UseSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound.UseSSO') | Specifies whether the HTTP adapter will issue the SSO ticket to messages that arrive on this receive location. |

| Methods | |
| :--- | :--- |
| [GetAddress()](HttpAdapter.Inbound.GetAddress().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound.GetAddress()') | |
| [GetPublicAddress()](HttpAdapter.Inbound.GetPublicAddress().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound.GetPublicAddress()') | |
| [Save(IPropertyBag)](HttpAdapter.Inbound.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | |
| [Validate()](HttpAdapter.Inbound.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound.Validate()') | |
