#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Xsl](Be.Stateless.BizTalk.Xml.Xsl.md 'Be.Stateless.BizTalk.Xml.Xsl').[XsltTranslatorBase](XsltTranslatorBase.md 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase')

## XsltTranslatorBase.CreateTranslatedRequestMessage(MessageVersion, string, XmlReader) Method

Creates the translated request [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message') using the specified [reader](XsltTranslatorBase.CreateTranslatedRequestMessage(MessageVersion,string,XmlReader).md#Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateTranslatedRequestMessage(System.ServiceModel.Channels.MessageVersion,string,System.Xml.XmlReader).reader 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateTranslatedRequestMessage(System.ServiceModel.Channels.MessageVersion, string, System.Xml.XmlReader).reader'), [action](XsltTranslatorBase.CreateTranslatedRequestMessage(MessageVersion,string,XmlReader).md#Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateTranslatedRequestMessage(System.ServiceModel.Channels.MessageVersion,string,System.Xml.XmlReader).action 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateTranslatedRequestMessage(System.ServiceModel.Channels.MessageVersion, string, System.Xml.XmlReader).action') and [version](XsltTranslatorBase.CreateTranslatedRequestMessage(MessageVersion,string,XmlReader).md#Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateTranslatedRequestMessage(System.ServiceModel.Channels.MessageVersion,string,System.Xml.XmlReader).version 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateTranslatedRequestMessage(System.ServiceModel.Channels.MessageVersion, string, System.Xml.XmlReader).version').

```csharp
protected virtual System.ServiceModel.Channels.Message CreateTranslatedRequestMessage(System.ServiceModel.Channels.MessageVersion version, string action, System.Xml.XmlReader reader);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateTranslatedRequestMessage(System.ServiceModel.Channels.MessageVersion,string,System.Xml.XmlReader).version'></a>

`version` [System.ServiceModel.Channels.MessageVersion](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.MessageVersion 'System.ServiceModel.Channels.MessageVersion')

A [System.ServiceModel.Channels.MessageVersion](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.MessageVersion 'System.ServiceModel.Channels.MessageVersion') object that specifies the SOAP version to use for the message. It defaults to the
version of the incoming [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') request; see [Version](XmlMessage.Version.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage.Version').

<a name='Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateTranslatedRequestMessage(System.ServiceModel.Channels.MessageVersion,string,System.Xml.XmlReader).action'></a>

`action` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

A description of how the message should be processed. It defaults to the action of the incoming [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') request; see [Action](XmlMessage.Action.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage.Action').

<a name='Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.CreateTranslatedRequestMessage(System.ServiceModel.Channels.MessageVersion,string,System.Xml.XmlReader).reader'></a>

`reader` [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')

The [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') object to be used for reading the SOAP message. It defaults to the output of the [RequestXslt](XsltTranslatorBase.RequestXslt.md 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase.RequestXslt') that has been applied to the body of the request [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage').

#### Returns
[System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')  
A [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message') object for the message created.