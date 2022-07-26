#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels](Be.Stateless.BizTalk.ServiceModel.Channels.md 'Be.Stateless.BizTalk.ServiceModel.Channels')

## IXmlMessageConverter Interface

Scaffolding interface meant to help the service relay, together made of the [ServiceRelay](ServiceRelay.md 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay') and its necessary
[Be.Stateless.BizTalk.ServiceModel.ClientRelay](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ServiceModel.ClientRelay 'Be.Stateless.BizTalk.ServiceModel.ClientRelay') counterpart, to convert [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')s back and forth to native generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message')s.

```csharp
public interface IXmlMessageConverter
```

Derived  
&#8627; [DefaultConverter](DefaultConverter.md 'Be.Stateless.BizTalk.ServiceModel.Channels.DefaultConverter')  
&#8627; [XsltTranslatorBase](XsltTranslatorBase.md 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase')

| Methods | |
| :--- | :--- |
| [CreateMessageRequestFromXmlRequest&lt;TRequest&gt;(TRequest)](IXmlMessageConverter.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).md 'Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter.CreateMessageRequestFromXmlRequest<TRequest>(TRequest)') | Converts an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to a generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message'). |
| [CreateXmlResponseFromMessageResponse&lt;TResponse&gt;(Message)](IXmlMessageConverter.CreateXmlResponseFromMessageResponse_TResponse_(Message).md 'Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter.CreateXmlResponseFromMessageResponse<TResponse>(System.ServiceModel.Channels.Message)') | Converts a generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message') to an an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage'). |
