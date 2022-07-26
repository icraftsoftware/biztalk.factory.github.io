#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Dispatcher](Be.Stateless.BizTalk.ServiceModel.Dispatcher.md 'Be.Stateless.BizTalk.ServiceModel.Dispatcher').[FaultMessageMinifier](FaultMessageMinifier.md 'Be.Stateless.BizTalk.ServiceModel.Dispatcher.FaultMessageMinifier')

## FaultMessageMinifier.AfterReceiveReply(Message, object) Method

Enables inspection or modification of a message after a reply message is received but prior to passing it back to the
client application.

```csharp
public void AfterReceiveReply(ref System.ServiceModel.Channels.Message reply, object correlationState);
```
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Dispatcher.FaultMessageMinifier.AfterReceiveReply(System.ServiceModel.Channels.Message,object).reply'></a>

`reply` [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')

The message to be transformed into types and handed back to the client application.

<a name='Be.Stateless.BizTalk.ServiceModel.Dispatcher.FaultMessageMinifier.AfterReceiveReply(System.ServiceModel.Channels.Message,object).correlationState'></a>

`correlationState` [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')

Correlation state data.

Implements [AfterReceiveReply(Message, object)](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Dispatcher.IClientMessageInspector.AfterReceiveReply#System_ServiceModel_Dispatcher_IClientMessageInspector_AfterReceiveReply_System_ServiceModel_Channels_Message@,System_Object_ 'System.ServiceModel.Dispatcher.IClientMessageInspector.AfterReceiveReply(System.ServiceModel.Channels.Message@,System.Object)')