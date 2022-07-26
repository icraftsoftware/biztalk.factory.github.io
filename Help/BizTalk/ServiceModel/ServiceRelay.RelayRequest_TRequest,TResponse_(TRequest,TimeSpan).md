#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel](Be.Stateless.BizTalk.ServiceModel.md 'Be.Stateless.BizTalk.ServiceModel').[ServiceRelay](ServiceRelay.md 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay')

## ServiceRelay.RelayRequest<TRequest,TResponse>(TRequest, TimeSpan) Method

Relays an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request and returns the correlated [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based response
within a specified interval of time.

```csharp
protected TResponse RelayRequest<TRequest,TResponse>(TRequest request, System.TimeSpan timeout)
    where TRequest : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage
    where TResponse : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,System.TimeSpan).TRequest'></a>

`TRequest`

The type of the [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request.

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,System.TimeSpan).TResponse'></a>

`TResponse`

The type of the [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based response.
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,System.TimeSpan).request'></a>

`request` [TRequest](ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,TimeSpan).md#Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,System.TimeSpan).TRequest 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest<TRequest,TResponse>(TRequest, System.TimeSpan).TRequest')

The [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request.

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,System.TimeSpan).timeout'></a>

`timeout` [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

The [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan') that specifies the interval of time within which a response must be received.

#### Returns
[TResponse](ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,TimeSpan).md#Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest_TRequest,TResponse_(TRequest,System.TimeSpan).TResponse 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay.RelayRequest<TRequest,TResponse>(TRequest, System.TimeSpan).TResponse')  
The [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based response.

### Remarks

If a timeout is passed while calling the function then that value is used. If the [System.ServiceModel.Channels.Binding.SendTimeout](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Binding.SendTimeout 'System.ServiceModel.Channels.Binding.SendTimeout')
is set on the binding, then the value on the binding is used if no timeout is specified while calling the function.

The [System.ServiceModel.Channels.ChannelBase.DefaultSendTimeout](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.ChannelBase.DefaultSendTimeout 'System.ServiceModel.Channels.ChannelBase.DefaultSendTimeout') is used if no timeout is specified on either the binding or while
calling the function. This default value is 1 minute.