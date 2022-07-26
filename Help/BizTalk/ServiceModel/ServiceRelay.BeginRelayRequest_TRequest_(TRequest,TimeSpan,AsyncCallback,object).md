#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel](Be.Stateless.BizTalk.ServiceModel.md 'Be.Stateless.BizTalk.ServiceModel').[ServiceRelay](ServiceRelay.md 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay')

## ServiceRelay.BeginRelayRequest<TRequest>(TRequest, TimeSpan, AsyncCallback, object) Method

Begins an asynchronous operation to relay an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request to the reply side of a
request-reply message exchange within a specified interval of time.

```csharp
protected System.IAsyncResult BeginRelayRequest<TRequest>(TRequest request, System.TimeSpan timeout, System.AsyncCallback asyncCallback, object asyncState)
    where TRequest : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest_TRequest_(TRequest,System.TimeSpan,System.AsyncCallback,object).TRequest'></a>

`TRequest`

The type of the [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request.
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest_TRequest_(TRequest,System.TimeSpan,System.AsyncCallback,object).request'></a>

`request` [TRequest](ServiceRelay.BeginRelayRequest_TRequest_(TRequest,TimeSpan,AsyncCallback,object).md#Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest_TRequest_(TRequest,System.TimeSpan,System.AsyncCallback,object).TRequest 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest<TRequest>(TRequest, System.TimeSpan, System.AsyncCallback, object).TRequest')

The [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request.

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest_TRequest_(TRequest,System.TimeSpan,System.AsyncCallback,object).timeout'></a>

`timeout` [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

The [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan') that specifies the interval of time within which a response must be received.

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest_TRequest_(TRequest,System.TimeSpan,System.AsyncCallback,object).asyncCallback'></a>

`asyncCallback` [System.AsyncCallback](https://docs.microsoft.com/en-us/dotnet/api/System.AsyncCallback 'System.AsyncCallback')

The [System.AsyncCallback](https://docs.microsoft.com/en-us/dotnet/api/System.AsyncCallback 'System.AsyncCallback') delegate that receives the notification of the completion of the asynchronous
operation transmitting a request message.

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest_TRequest_(TRequest,System.TimeSpan,System.AsyncCallback,object).asyncState'></a>

`asyncState` [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')

An object, specified by the application, that contains state information associated with the asynchronous operation
transmitting a request message.

#### Returns
[System.IAsyncResult](https://docs.microsoft.com/en-us/dotnet/api/System.IAsyncResult 'System.IAsyncResult')  
The [System.IAsyncResult](https://docs.microsoft.com/en-us/dotnet/api/System.IAsyncResult 'System.IAsyncResult') that references the asynchronous message transmission.

### Remarks

If a timeout is passed while calling the function then that value is used. If the [System.ServiceModel.Channels.Binding.SendTimeout](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Binding.SendTimeout 'System.ServiceModel.Channels.Binding.SendTimeout')
is set on the binding, then the value on the binding is used if no timeout is specified while calling the function.

The [System.ServiceModel.Channels.ChannelBase.DefaultSendTimeout](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.ChannelBase.DefaultSendTimeout 'System.ServiceModel.Channels.ChannelBase.DefaultSendTimeout') is used if no timeout is specified on either the binding or while
calling the function. This default value is 1 minute.