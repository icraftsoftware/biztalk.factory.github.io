#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Xsl](Be.Stateless.BizTalk.Xml.Xsl.md 'Be.Stateless.BizTalk.Xml.Xsl').[XsltTranslatorBase](XsltTranslatorBase.md 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase')

## XsltTranslatorBase.CreateMessageRequestFromXmlRequest<TRequest>(TRequest) Method

Translates an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to a generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message').

```csharp
public virtual System.ServiceModel.Channels.Message CreateMessageRequestFromXmlRequest<TRequest>(TRequest xmlRequest)
    where TRequest : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).TRequest'></a>

`TRequest`

The type of the [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to translate.
#### Parameters

<a name='Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).xmlRequest'></a>

`xmlRequest` [TRequest](XsltTranslatorBase.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).md#Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).TRequest 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateMessageRequestFromXmlRequest<TRequest>(TRequest).TRequest')

The [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to translate.

Implements [CreateMessageRequestFromXmlRequest&lt;TRequest&gt;(TRequest)](IXmlMessageConverter.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).md 'Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter.CreateMessageRequestFromXmlRequest<TRequest>(TRequest)')

#### Returns
[System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')  
The translated generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message').