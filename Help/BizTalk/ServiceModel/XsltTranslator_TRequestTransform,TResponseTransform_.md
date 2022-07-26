#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Xsl](Be.Stateless.BizTalk.Xml.Xsl.md 'Be.Stateless.BizTalk.Xml.Xsl')

## XsltTranslator<TRequestTransform,TResponseTransform> Class

Translates [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')s back and forth to native generic WCF [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')s by applying an [System.Xml.Xsl.XslCompiledTransform](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XslCompiledTransform 'System.Xml.Xsl.XslCompiledTransform') to their payloads.

```csharp
public class XsltTranslator<TRequestTransform,TResponseTransform> : Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase
    where TRequestTransform : Be.Stateless.BizTalk.Xml.Xsl.XsltTransformBase, new()
    where TResponseTransform : Be.Stateless.BizTalk.Xml.Xsl.XsltTransformBase, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Xml.Xsl.XsltTranslator_TRequestTransform,TResponseTransform_.TRequestTransform'></a>

`TRequestTransform`

<a name='Be.Stateless.BizTalk.Xml.Xsl.XsltTranslator_TRequestTransform,TResponseTransform_.TResponseTransform'></a>

`TResponseTransform`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [XsltTranslatorBase](XsltTranslatorBase.md 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase') &#129106; XsltTranslator<TRequestTransform,TResponseTransform>

Derived  
&#8627; [CompositeXsltTranslator&lt;TRequestTransform,TResponseTransform&gt;](CompositeXsltTranslator_TRequestTransform,TResponseTransform_.md 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator<TRequestTransform,TResponseTransform>')

| Properties | |
| :--- | :--- |
| [RequestXslt](XsltTranslator_TRequestTransform,TResponseTransform_.RequestXslt.md 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslator<TRequestTransform,TResponseTransform>.RequestXslt') | [System.Xml.Xsl.XslCompiledTransform](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XslCompiledTransform 'System.Xml.Xsl.XslCompiledTransform') to apply to the request [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')'s body. |
| [ResponseXslt](XsltTranslator_TRequestTransform,TResponseTransform_.ResponseXslt.md 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslator<TRequestTransform,TResponseTransform>.ResponseXslt') | [System.Xml.Xsl.XslCompiledTransform](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XslCompiledTransform 'System.Xml.Xsl.XslCompiledTransform') to apply to get the response [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')'s body. |
