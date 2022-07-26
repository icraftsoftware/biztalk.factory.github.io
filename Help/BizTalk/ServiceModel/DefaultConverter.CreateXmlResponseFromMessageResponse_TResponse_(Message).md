#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels](Be.Stateless.BizTalk.ServiceModel.Channels.md 'Be.Stateless.BizTalk.ServiceModel.Channels').[DefaultConverter](DefaultConverter.md 'Be.Stateless.BizTalk.ServiceModel.Channels.DefaultConverter')

## DefaultConverter.CreateXmlResponseFromMessageResponse<TResponse>(Message) Method

Converts a generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message') to an an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage').

```csharp
public TResponse CreateXmlResponseFromMessageResponse<TResponse>(System.ServiceModel.Channels.Message response)
    where TResponse : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.DefaultConverter.CreateXmlResponseFromMessageResponse_TResponse_(System.ServiceModel.Channels.Message).TResponse'></a>

`TResponse`

The type of the resulting converted [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage').
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.DefaultConverter.CreateXmlResponseFromMessageResponse_TResponse_(System.ServiceModel.Channels.Message).response'></a>

`response` [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')

The generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message') to convert.

Implements [CreateXmlResponseFromMessageResponse&lt;TResponse&gt;(Message)](IXmlMessageConverter.CreateXmlResponseFromMessageResponse_TResponse_(Message).md 'Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter.CreateXmlResponseFromMessageResponse<TResponse>(System.ServiceModel.Channels.Message)')

#### Returns
[TResponse](DefaultConverter.CreateXmlResponseFromMessageResponse_TResponse_(Message).md#Be.Stateless.BizTalk.ServiceModel.Channels.DefaultConverter.CreateXmlResponseFromMessageResponse_TResponse_(System.ServiceModel.Channels.Message).TResponse 'Be.Stateless.BizTalk.ServiceModel.Channels.DefaultConverter.CreateXmlResponseFromMessageResponse<TResponse>(System.ServiceModel.Channels.Message).TResponse')  
The converted [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage').