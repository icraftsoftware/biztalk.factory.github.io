#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Channels](Be.Stateless.BizTalk.Unit.ServiceModel.Channels.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels').[IMessageService](IMessageService.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService')

## IMessageService.Invoke(Message) Method

Sends a [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')-based request and returns the correlated [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')-based response.

```csharp
System.ServiceModel.Channels.Message Invoke(System.ServiceModel.Channels.Message request);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService.Invoke(System.ServiceModel.Channels.Message).request'></a>

`request` [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')

The request [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message') to be transmitted.

#### Returns
[System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')  
The [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message') received in response to the request.