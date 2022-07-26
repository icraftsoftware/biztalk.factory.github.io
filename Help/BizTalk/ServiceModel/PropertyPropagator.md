#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Dispatcher](Be.Stateless.BizTalk.ServiceModel.Dispatcher.md 'Be.Stateless.BizTalk.ServiceModel.Dispatcher')

## PropertyPropagator Class

WCF behavior that either propagates or promotes BizTalk message context properties from request to response.

```csharp
public class PropertyPropagator :
System.ServiceModel.Dispatcher.IClientMessageInspector
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; PropertyPropagator

Implements [System.ServiceModel.Dispatcher.IClientMessageInspector](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Dispatcher.IClientMessageInspector 'System.ServiceModel.Dispatcher.IClientMessageInspector')

### See Also
- [https://docs.microsoft.com/en-us/biztalk/core/soap-headers-with-published-wcf-services](https://docs.microsoft.com/en-us/biztalk/core/soap-headers-with-published-wcf-services 'https://docs.microsoft.com/en-us/biztalk/core/soap-headers-with-published-wcf-services')
- [https://adventuresinsidethemessagebox.wordpress.com/2015/07/01/sharing-context-between-biztalk-and-wcf-behavior-extensions/](https://adventuresinsidethemessagebox.wordpress.com/2015/07/01/sharing-context-between-biztalk-and-wcf-behavior-extensions/ 'https://adventuresinsidethemessagebox.wordpress.com/2015/07/01/sharing-context-between-biztalk-and-wcf-behavior-extensions/')

| Constructors | |
| :--- | :--- |
| [PropertyPropagator(PropertyPropagationCollection)](PropertyPropagator.PropertyPropagator(PropertyPropagationCollection).md 'Be.Stateless.BizTalk.ServiceModel.Dispatcher.PropertyPropagator.PropertyPropagator(Be.Stateless.BizTalk.ServiceModel.Configuration.PropertyPropagationCollection)') | |

| Methods | |
| :--- | :--- |
| [AfterReceiveReply(Message, object)](PropertyPropagator.AfterReceiveReply(Message,object).md 'Be.Stateless.BizTalk.ServiceModel.Dispatcher.PropertyPropagator.AfterReceiveReply(System.ServiceModel.Channels.Message, object)') | |
| [BeforeSendRequest(Message, IClientChannel)](PropertyPropagator.BeforeSendRequest(Message,IClientChannel).md 'Be.Stateless.BizTalk.ServiceModel.Dispatcher.PropertyPropagator.BeforeSendRequest(System.ServiceModel.Channels.Message, System.ServiceModel.IClientChannel)') | |
