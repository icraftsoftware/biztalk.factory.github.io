#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Xsl](Be.Stateless.BizTalk.Xml.Xsl.md 'Be.Stateless.BizTalk.Xml.Xsl').[CompositeXsltTranslator&lt;TRequestTransform,TResponseTransform&gt;](CompositeXsltTranslator_TRequestTransform,TResponseTransform_.md 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator<TRequestTransform,TResponseTransform>')

## CompositeXsltTranslator<TRequestTransform,TResponseTransform>.CreateMessageRequestFromXmlRequest<TRequest>(TRequest) Method

Translates an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to a generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message').

```csharp
public override System.ServiceModel.Channels.Message CreateMessageRequestFromXmlRequest<TRequest>(TRequest xmlRequest)
    where TRequest : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator_TRequestTransform,TResponseTransform_.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).TRequest'></a>

`TRequest`

The type of the [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to translate.
#### Parameters

<a name='Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator_TRequestTransform,TResponseTransform_.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).xmlRequest'></a>

`xmlRequest` [TRequest](CompositeXsltTranslator_TRequestTransform,TResponseTransform_.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).md#Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator_TRequestTransform,TResponseTransform_.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).TRequest 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator<TRequestTransform,TResponseTransform>.CreateMessageRequestFromXmlRequest<TRequest>(TRequest).TRequest')

The [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to translate.

Implements [CreateMessageRequestFromXmlRequest&lt;TRequest&gt;(TRequest)](IXmlMessageConverter.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).md 'Be.Stateless.BizTalk.ServiceModel.Channels.IXmlMessageConverter.CreateMessageRequestFromXmlRequest<TRequest>(TRequest)')

#### Returns
[System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')  
The translated generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message').

### Remarks
It grabs a reference to the incoming [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-derived request before delegating to base class.