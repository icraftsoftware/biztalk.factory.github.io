#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Xsl](Be.Stateless.BizTalk.Xml.Xsl.md 'Be.Stateless.BizTalk.Xml.Xsl').[XsltTranslatorBase](XsltTranslatorBase.md 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase')

## XsltTranslatorBase.CreateXmlResponseFromMessageResponse<TResponse>(Message) Method

Translates a generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message') to an an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage').

```csharp
public virtual TResponse CreateXmlResponseFromMessageResponse<TResponse>(System.ServiceModel.Channels.Message response)
    where TResponse : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateXmlResponseFromMessageResponse_TResponse_(System.ServiceModel.Channels.Message).TResponse'></a>

`TResponse`

The type of the resulting translated [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage').
#### Parameters

<a name='Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateXmlResponseFromMessageResponse_TResponse_(System.ServiceModel.Channels.Message).response'></a>

`response` [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')

The generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message') to translate.

Implements [CreateXmlResponseFromMessageResponse&lt;TResponse&gt;(Message)](IXmlMessageConverter.CreateXmlResponseFromMessageResponse_TResponse_(Message).md 'Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter.CreateXmlResponseFromMessageResponse<TResponse>(System.ServiceModel.Channels.Message)')

#### Returns
[TResponse](XsltTranslatorBase.CreateXmlResponseFromMessageResponse_TResponse_(Message).md#Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateXmlResponseFromMessageResponse_TResponse_(System.ServiceModel.Channels.Message).TResponse 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateXmlResponseFromMessageResponse<TResponse>(System.ServiceModel.Channels.Message).TResponse')  
The translated [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage').