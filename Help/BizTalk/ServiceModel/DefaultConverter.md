#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels](Be.Stateless.BizTalk.ServiceModel.Channels.md 'Be.Stateless.BizTalk.ServiceModel.Channels')

## DefaultConverter Class

A default [IXmlMessageConverter](IXmlMessageConverter.md 'Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter') converter that merely converts from an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to a
generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message') and back.

```csharp
public class DefaultConverter :
Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; DefaultConverter

Implements [IXmlMessageConverter](IXmlMessageConverter.md 'Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter')

### Remarks
This class acts as a mere converter and consequently does not translate any of the message's SOAP [System.ServiceModel.Channels.MessageVersion](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.MessageVersion 'System.ServiceModel.Channels.MessageVersion'), action, or payload/body.

| Properties | |
| :--- | :--- |
| [Instance](DefaultConverter.Instance.md 'Be.Stateless.BizTalk.ServiceModel.Channels.DefaultConverter.Instance') | Singleton instance |

| Methods | |
| :--- | :--- |
| [CreateMessageRequestFromXmlRequest&lt;TRequest&gt;(TRequest)](DefaultConverter.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).md 'Be.Stateless.BizTalk.ServiceModel.Channels.DefaultConverter.CreateMessageRequestFromXmlRequest<TRequest>(TRequest)') | Converts an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to its [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message') equivalent. |
| [CreateXmlResponseFromMessageResponse&lt;TResponse&gt;(Message)](DefaultConverter.CreateXmlResponseFromMessageResponse_TResponse_(Message).md 'Be.Stateless.BizTalk.ServiceModel.Channels.DefaultConverter.CreateXmlResponseFromMessageResponse<TResponse>(System.ServiceModel.Channels.Message)') | Converts a generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message') to an an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage'). |
