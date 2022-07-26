#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Xsl](Be.Stateless.BizTalk.Xml.Xsl.md 'Be.Stateless.BizTalk.Xml.Xsl').[XsltTranslatorBase](XsltTranslatorBase.md 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase')

## XsltTranslatorBase.BuildTranslatedResponseXmlMessage(XmlMessage, XmlReader) Method

Loads an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')'s translated XML representation.

```csharp
protected virtual void BuildTranslatedResponseXmlMessage(Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage xmlResponse, System.Xml.XmlReader xmlReader);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.BuildTranslatedResponseXmlMessage(Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage,System.Xml.XmlReader).xmlResponse'></a>

`xmlResponse` [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')

The [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to load XML content into.

<a name='Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.BuildTranslatedResponseXmlMessage(Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage,System.Xml.XmlReader).xmlReader'></a>

`xmlReader` [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')

The XML content to load.