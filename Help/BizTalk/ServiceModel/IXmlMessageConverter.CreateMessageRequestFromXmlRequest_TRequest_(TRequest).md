#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels](Be.Stateless.BizTalk.ServiceModel.Channels.md 'Be.Stateless.BizTalk.ServiceModel.Channels').[IXmlMessageConverter](IXmlMessageConverter.md 'Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter')

## IXmlMessageConverter.CreateMessageRequestFromXmlRequest<TRequest>(TRequest) Method

Converts an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to a generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message').

```csharp
System.ServiceModel.Channels.Message CreateMessageRequestFromXmlRequest<TRequest>(TRequest xmlRequest)
    where TRequest : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).TRequest'></a>

`TRequest`

The type of the [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to convert.
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).xmlRequest'></a>

`xmlRequest` [TRequest](IXmlMessageConverter.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).md#Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).TRequest 'Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter.CreateMessageRequestFromXmlRequest<TRequest>(TRequest).TRequest')

The [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to convert.

#### Returns
[System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')  
The converted generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message').