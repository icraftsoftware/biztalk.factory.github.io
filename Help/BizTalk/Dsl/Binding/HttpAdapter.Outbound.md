#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter')

## HttpAdapter.Outbound Class

You use the HTTP adapter to exchange information between Microsoft BizTalk Server and an application by means of the
HTTP protocol. HTTP is the primary protocol for inter-business message exchange. Applications can send messages to a
server by sending HTTP POST or HTTP GET requests to a specified HTTP URL. The HTTP adapter receives the HTTP requests
and submits them to BizTalk Server for processing. Similarly, BizTalk Server can transmit messages to remote
applications by sending HTTP POST requests to a specified HTTP URL.

```csharp
public class HttpAdapter.Outbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IOutboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundCredentials,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter') &#129106; Outbound

Implements [IOutboundAdapter](IOutboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IOutboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation'), [IAdapterConfigOutboundCredentials](IAdapterConfigOutboundCredentials.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundCredentials'), [IAdapterConfigSSO](IAdapterConfigSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO')

### See Also
- [HTTP Adapter](https://docs.microsoft.com/en-us/biztalk/core/http-adapter 'https://docs.microsoft.com/en-us/biztalk/core/http-adapter')
- [Configuring the HTTP Adapter](https://docs.microsoft.com/en-us/biztalk/core/configuring-the-http-adapter 'https://docs.microsoft.com/en-us/biztalk/core/configuring-the-http-adapter')
- [HTTP Send Adapter](https://docs.microsoft.com/en-us/biztalk/core/http-send-adapter 'https://docs.microsoft.com/en-us/biztalk/core/http-send-adapter')
- [How to Configure an HTTP Send Handler](https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-an-http-send-handler 'https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-an-http-send-handler')
- [How to Configure an HTTP Send Port](https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-an-http-send-port 'https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-an-http-send-port')
- [Restrictions on the Destination URL Property](https://docs.microsoft.com/en-us/biztalk/core/restrictions-on-the-destination-url-property 'https://docs.microsoft.com/en-us/biztalk/core/restrictions-on-the-destination-url-property')

| Constructors | |
| :--- | :--- |
| [Outbound()](HttpAdapter.Outbound.Outbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.Outbound()') | |
| [Outbound(Action&lt;Outbound&gt;)](HttpAdapter.Outbound.Outbound(Action_Outbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.Outbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound>)') | |

| Properties | |
| :--- | :--- |
| [AffiliateApplicationName](HttpAdapter.Outbound.AffiliateApplicationName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.AffiliateApplicationName') | Name of the affiliate application to use for SSO. |
| [AuthenticationScheme](HttpAdapter.Outbound.AuthenticationScheme.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.AuthenticationScheme') | Type of authentication to use with the destination server. |
| [Certificate](HttpAdapter.Outbound.Certificate.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.Certificate') | Specify the thumbprint of the client certificate to use for establishing a Secure Sockets Layer (SSL) connection. |
| [ContentType](HttpAdapter.Outbound.ContentType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.ContentType') | Content type of the request messages. |
| [EnableChunkedEncoding](HttpAdapter.Outbound.EnableChunkedEncoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.EnableChunkedEncoding') | Specifies whether or not chunked encoding is used by the HTTP adapter. |
| [MaxRedirects](HttpAdapter.Outbound.MaxRedirects.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.MaxRedirects') | Maximum number of times that the HTTP adapter can redirect the request. |
| [Password](HttpAdapter.Outbound.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.Password') | User password to use for authentication with the server. |
| [ProxyName](HttpAdapter.Outbound.ProxyName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.ProxyName') | Specifies the proxy server name. |
| [ProxyPassword](HttpAdapter.Outbound.ProxyPassword.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.ProxyPassword') | Specifies the user password for authentication with the proxy server. |
| [ProxyPort](HttpAdapter.Outbound.ProxyPort.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.ProxyPort') | Specifies the proxy server port. |
| [ProxyUserName](HttpAdapter.Outbound.ProxyUserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.ProxyUserName') | Specifies the user name for authentication with the proxy server. |
| [RequestTimeout](HttpAdapter.Outbound.RequestTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.RequestTimeout') | Specify the time-out for the HTTP/HTTPS transmission. If the HTTP adapter does not receive the response within this time, the service logs the error and resubmits the message based on the retry infrastructure. |
| [Url](HttpAdapter.Outbound.Url.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.Url') | Specify the address to send HTTP requests. Include query strings appended to the base URL. |
| [UseHandlerProxySettings](HttpAdapter.Outbound.UseHandlerProxySettings.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.UseHandlerProxySettings') | Specifies whether the HTTP send port will use the proxy configuration for the send handler. |
| [UseProxy](HttpAdapter.Outbound.UseProxy.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.UseProxy') | Specifies whether the HTTP adapter will use the proxy server. The proxy server can be shared by all HTTP send ports. |
| [UserName](HttpAdapter.Outbound.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.UserName') | User name to use for authentication with the server. |
| [UseSSO](HttpAdapter.Outbound.UseSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.UseSSO') | Specifies if SSO will be used for the send port. |

| Methods | |
| :--- | :--- |
| [GetAddress()](HttpAdapter.Outbound.GetAddress().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.GetAddress()') | |
| [Save(IPropertyBag)](HttpAdapter.Outbound.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | |
| [Validate()](HttpAdapter.Outbound.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound.Validate()') | |
