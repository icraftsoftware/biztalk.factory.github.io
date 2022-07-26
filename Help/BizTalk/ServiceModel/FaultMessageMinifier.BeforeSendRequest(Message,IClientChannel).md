#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Dispatcher](Be.Stateless.BizTalk.ServiceModel.Dispatcher.md 'Be.Stateless.BizTalk.ServiceModel.Dispatcher').[FaultMessageMinifier](FaultMessageMinifier.md 'Be.Stateless.BizTalk.ServiceModel.Dispatcher.FaultMessageMinifier')

## FaultMessageMinifier.BeforeSendRequest(Message, IClientChannel) Method

Enables inspection or modification of a message before a request message is sent to a service.

```csharp
public object BeforeSendRequest(ref System.ServiceModel.Channels.Message request, System.ServiceModel.IClientChannel channel);
```
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Dispatcher.FaultMessageMinifier.BeforeSendRequest(System.ServiceModel.Channels.Message,System.ServiceModel.IClientChannel).request'></a>

`request` [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')

The message to be sent to the service.

<a name='Be.Stateless.BizTalk.ServiceModel.Dispatcher.FaultMessageMinifier.BeforeSendRequest(System.ServiceModel.Channels.Message,System.ServiceModel.IClientChannel).channel'></a>

`channel` [System.ServiceModel.IClientChannel](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.IClientChannel 'System.ServiceModel.IClientChannel')

The  client object channel.

Implements [BeforeSendRequest(Message, IClientChannel)](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Dispatcher.IClientMessageInspector.BeforeSendRequest#System_ServiceModel_Dispatcher_IClientMessageInspector_BeforeSendRequest_System_ServiceModel_Channels_Message@,System_ServiceModel_IClientChannel_ 'System.ServiceModel.Dispatcher.IClientMessageInspector.BeforeSendRequest(System.ServiceModel.Channels.Message@,System.ServiceModel.IClientChannel)')

#### Returns
[System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')  
The object that is returned as the <i>correlationState</i> argument of the [System.ServiceModel.Dispatcher.IClientMessageInspector.AfterReceiveReply(System.ServiceModel.Channels.Message@,System.Object)](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Dispatcher.IClientMessageInspector.AfterReceiveReply#System_ServiceModel_Dispatcher_IClientMessageInspector_AfterReceiveReply_System_ServiceModel_Channels_Message@,System_Object_ 'System.ServiceModel.Dispatcher.IClientMessageInspector.AfterReceiveReply(System.ServiceModel.Channels.Message@,System.Object)') method. This is null if no correlation state is used. The best
practice is to make this a [System.Guid](https://docs.microsoft.com/en-us/dotnet/api/System.Guid 'System.Guid') to ensure that no two <i>correlationState</i> objects are the same.