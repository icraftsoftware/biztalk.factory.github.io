#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels](Be.Stateless.BizTalk.ServiceModel.Channels.md 'Be.Stateless.BizTalk.ServiceModel.Channels').[DefaultConverter](DefaultConverter.md 'Be.Stateless.BizTalk.ServiceModel.Channels.DefaultConverter')

## DefaultConverter.CreateMessageRequestFromXmlRequest<TRequest>(TRequest) Method

Converts an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to its [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message') equivalent.

```csharp
public System.ServiceModel.Channels.Message CreateMessageRequestFromXmlRequest<TRequest>(TRequest xmlRequest)
    where TRequest : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.DefaultConverter.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).TRequest'></a>

`TRequest`

The type of the [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to convert.
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.DefaultConverter.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).xmlRequest'></a>

`xmlRequest` [TRequest](DefaultConverter.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).md#Be.Stateless.BizTalk.ServiceModel.Channels.DefaultConverter.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).TRequest 'Be.Stateless.BizTalk.ServiceModel.Channels.DefaultConverter.CreateMessageRequestFromXmlRequest<TRequest>(TRequest).TRequest')

The [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to convert.

Implements [CreateMessageRequestFromXmlRequest&lt;TRequest&gt;(TRequest)](IXmlMessageConverter.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).md 'Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter.CreateMessageRequestFromXmlRequest<TRequest>(TRequest)')

#### Returns
[System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')  
The converted WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message').