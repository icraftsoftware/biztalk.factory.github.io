#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel](Be.Stateless.BizTalk.ServiceModel.md 'Be.Stateless.BizTalk.ServiceModel').[ServiceRelay](ServiceRelay.md 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay')

## ServiceRelay.RelayRequest<TRequest,TResponse>(TRequest) Method

Relays an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request and returns the correlated [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based response.

```csharp
protected TResponse RelayRequest<TRequest,TResponse>(TRequest request)
    where TRequest : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage
    where TResponse : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest).TRequest'></a>

`TRequest`

The type of the [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request.

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest).TResponse'></a>

`TResponse`

The type of the [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based response.
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest).request'></a>

`request` [TRequest](ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest).md#Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest).TRequest 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest<TRequest,TResponse>(TRequest).TRequest')

The [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request.

#### Returns
[TResponse](ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest).md#Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest).TResponse 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest<TRequest,TResponse>(TRequest).TResponse')  
The [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based response.