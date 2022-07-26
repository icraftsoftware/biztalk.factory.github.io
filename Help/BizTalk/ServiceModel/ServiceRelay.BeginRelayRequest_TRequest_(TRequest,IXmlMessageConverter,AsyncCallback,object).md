#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel](Be.Stateless.BizTalk.ServiceModel.md 'Be.Stateless.BizTalk.ServiceModel').[ServiceRelay](ServiceRelay.md 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay')

## ServiceRelay.BeginRelayRequest<TRequest>(TRequest, IXmlMessageConverter, AsyncCallback, object) Method

Begins an asynchronous operation to convert and relay an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request to the reply side of
a request-reply message exchange.

```csharp
protected System.IAsyncResult BeginRelayRequest<TRequest>(TRequest request, Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter converter, System.AsyncCallback asyncCallback, object asyncState)
    where TRequest : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest_TRequest_(TRequest,Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter,System.AsyncCallback,object).TRequest'></a>

`TRequest`

The type of the [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request.
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest_TRequest_(TRequest,Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter,System.AsyncCallback,object).request'></a>

`request` [TRequest](ServiceRelay.BeginRelayRequest_TRequest_(TRequest,IXmlMessageConverter,AsyncCallback,object).md#Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest_TRequest_(TRequest,Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter,System.AsyncCallback,object).TRequest 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest<TRequest>(TRequest, Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter, System.AsyncCallback, object).TRequest')

The [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request to convert and relay.

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest_TRequest_(TRequest,Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter,System.AsyncCallback,object).converter'></a>

`converter` [IXmlMessageConverter](IXmlMessageConverter.md 'Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter')

The [IXmlMessageConverter](IXmlMessageConverter.md 'Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter') to use to convert the request and response.

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest_TRequest_(TRequest,Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter,System.AsyncCallback,object).asyncCallback'></a>

`asyncCallback` [System.AsyncCallback](https://docs.microsoft.com/en-us/dotnet/api/System.AsyncCallback 'System.AsyncCallback')

The [System.AsyncCallback](https://docs.microsoft.com/en-us/dotnet/api/System.AsyncCallback 'System.AsyncCallback') delegate that receives the notification of the completion of the asynchronous
operation transmitting a request message.

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest_TRequest_(TRequest,Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter,System.AsyncCallback,object).asyncState'></a>

`asyncState` [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')

An object, specified by the application, that contains state information associated with the asynchronous operation
transmitting a request message.

#### Returns
[System.IAsyncResult](https://docs.microsoft.com/en-us/dotnet/api/System.IAsyncResult 'System.IAsyncResult')  
The [System.IAsyncResult](https://docs.microsoft.com/en-us/dotnet/api/System.IAsyncResult 'System.IAsyncResult') that references the asynchronous message transmission.