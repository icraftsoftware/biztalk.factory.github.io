#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Dispatcher](Be.Stateless.BizTalk.ServiceModel.Dispatcher.md 'Be.Stateless.BizTalk.ServiceModel.Dispatcher')

## FaultMessageMinifier Class

Remove security header from fault message so that, when a fault message is serialized, the actual fault reason is not
truncated away due to the lengthy security headers.

```csharp
public class FaultMessageMinifier :
System.ServiceModel.Dispatcher.IClientMessageInspector
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; FaultMessageMinifier

Implements [System.ServiceModel.Dispatcher.IClientMessageInspector](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Dispatcher.IClientMessageInspector 'System.ServiceModel.Dispatcher.IClientMessageInspector')

### See Also
- [http://weblogs.asp.net/paolopia/archive/2008/02/25/handling-custom-soap-headers-via-wcf-behaviors.aspx](http://weblogs.asp.net/paolopia/archive/2008/02/25/handling-custom-soap-headers-via-wcf-behaviors.aspx 'http://weblogs.asp.net/paolopia/archive/2008/02/25/handling-custom-soap-headers-via-wcf-behaviors.aspx')
- [https://docs.microsoft.com/en-us/dotnet/framework/wcf/samples/message-inspectors](https://docs.microsoft.com/en-us/dotnet/framework/wcf/samples/message-inspectors 'https://docs.microsoft.com/en-us/dotnet/framework/wcf/samples/message-inspectors')

| Methods | |
| :--- | :--- |
| [AfterReceiveReply(Message, object)](FaultMessageMinifier.AfterReceiveReply(Message,object).md 'Be.Stateless.BizTalk.ServiceModel.Dispatcher.FaultMessageMinifier.AfterReceiveReply(System.ServiceModel.Channels.Message, object)') | Enables inspection or modification of a message after a reply message is received but prior to passing it back to the client application. |
| [BeforeSendRequest(Message, IClientChannel)](FaultMessageMinifier.BeforeSendRequest(Message,IClientChannel).md 'Be.Stateless.BizTalk.ServiceModel.Dispatcher.FaultMessageMinifier.BeforeSendRequest(System.ServiceModel.Channels.Message, System.ServiceModel.IClientChannel)') | Enables inspection or modification of a message before a request message is sent to a service. |
