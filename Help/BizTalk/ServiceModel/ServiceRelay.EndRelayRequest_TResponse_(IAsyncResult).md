#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel](Be.Stateless.BizTalk.ServiceModel.md 'Be.Stateless.BizTalk.ServiceModel').[ServiceRelay](ServiceRelay.md 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay')

## ServiceRelay.EndRelayRequest<TResponse>(IAsyncResult) Method

Completes an asynchronous operation to return a, possibly converted, [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based response to a
relayed [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based request.

```csharp
protected TResponse EndRelayRequest<TResponse>(System.IAsyncResult asyncResult)
    where TResponse : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.EndRelayRequest_TResponse_(System.IAsyncResult).TResponse'></a>

`TResponse`

The type of the [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based response.
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.ServiceRelay.EndRelayRequest_TResponse_(System.IAsyncResult).asyncResult'></a>

`asyncResult` [System.IAsyncResult](https://docs.microsoft.com/en-us/dotnet/api/System.IAsyncResult 'System.IAsyncResult')

The [System.IAsyncResult](https://docs.microsoft.com/en-us/dotnet/api/System.IAsyncResult 'System.IAsyncResult') returned by a call to the [BeginRelayRequest&lt;TRequest&gt;(TRequest, AsyncCallback, object)](ServiceRelay.BeginRelayRequest_TRequest_(TRequest,AsyncCallback,object).md 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest<TRequest>(TRequest, System.AsyncCallback, object)') method.

#### Returns
[TResponse](ServiceRelay.EndRelayRequest_TResponse_(IAsyncResult).md#Be.Stateless.BizTalk.ServiceModel.ServiceRelay.EndRelayRequest_TResponse_(System.IAsyncResult).TResponse 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay.EndRelayRequest<TResponse>(System.IAsyncResult).TResponse')  
The [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-based response.