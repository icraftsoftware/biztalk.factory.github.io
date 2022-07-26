#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel](Be.Stateless.BizTalk.ServiceModel.md 'Be.Stateless.BizTalk.ServiceModel').[ServiceRelay](ServiceRelay.md 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay')

## ServiceRelay.RelayRequest<TRequest,TResponse>(TRequest, IXmlMessageConverter) Method

Converts and relays an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request and, converts and returns the correlated [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based response.

```csharp
protected TResponse RelayRequest<TRequest,TResponse>(TRequest request, Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter converter)
    where TRequest : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage
    where TResponse : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter).TRequest'></a>

`TRequest`

The type of the [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request.

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter).TResponse'></a>

`TResponse`

The type of the [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based response.
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter).request'></a>

`request` [TRequest](ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,IXmlMessageConverter).md#Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter).TRequest 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest<TRequest,TResponse>(TRequest, Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter).TRequest')

The [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request to convert and relay.

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter).converter'></a>

`converter` [IXmlMessageConverter](IXmlMessageConverter.md 'Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter')

The [IXmlMessageConverter](IXmlMessageConverter.md 'Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter') to use to convert the request and response.

#### Returns
[TResponse](ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,IXmlMessageConverter).md#Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter).TResponse 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest<TRequest,TResponse>(TRequest, Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter).TResponse')  
The converted [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based response.