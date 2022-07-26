#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Xsl](Be.Stateless.BizTalk.Xml.Xsl.md 'Be.Stateless.BizTalk.Xml.Xsl')

## CompositeXsltTranslator<TRequestTransform,TResponseTransform> Class

Translates [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')s back and forth to native generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message')s by applying an [System.Xml.Xsl.XslCompiledTransform](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XslCompiledTransform 'System.Xml.Xsl.XslCompiledTransform') to their payloads.

```csharp
public class CompositeXsltTranslator<TRequestTransform,TResponseTransform> : Be.Stateless.BizTalk.Xml.Xsl.XsltTranslator<TRequestTransform, TResponseTransform>
    where TRequestTransform : Be.Stateless.BizTalk.Xml.Xsl.XsltTransformBase, new()
    where TResponseTransform : Be.Stateless.BizTalk.Xml.Xsl.XsltTransformBase, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TRequestTransform'></a>

`TRequestTransform`

<a name='Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TResponseTransform'></a>

`TResponseTransform`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [XsltTranslatorBase](XsltTranslatorBase.md 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase') &#129106; [Be.Stateless.BizTalk.Xml.Xsl.XsltTranslator&lt;](XsltTranslator_TRequestTransform,TResponseTransform_.md 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslator<TRequestTransform,TResponseTransform>')[TRequestTransform](CompositeXsltTranslator_TRequestTransform,TResponseTransform_.md#Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TRequestTransform 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator<TRequestTransform,TResponseTransform>.TRequestTransform')[,](XsltTranslator_TRequestTransform,TResponseTransform_.md 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslator<TRequestTransform,TResponseTransform>')[TResponseTransform](CompositeXsltTranslator_TRequestTransform,TResponseTransform_.md#Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TResponseTransform 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator<TRequestTransform,TResponseTransform>.TResponseTransform')[&gt;](XsltTranslator_TRequestTransform,TResponseTransform_.md 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslator<TRequestTransform,TResponseTransform>') &#129106; CompositeXsltTranslator<TRequestTransform,TResponseTransform>

| Methods | |
| :--- | :--- |
| [CreateMessageRequestFromXmlRequest&lt;TRequest&gt;(TRequest)](CompositeXsltTranslator_TRequestTransform,TResponseTransform_.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).md 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator<TRequestTransform,TResponseTransform>.CreateMessageRequestFromXmlRequest<TRequest>(TRequest)') | Translates an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to a generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message'). |
| [TranslateResponse(XmlReader, XmlWriter)](CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(XmlReader,XmlWriter).md 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator<TRequestTransform,TResponseTransform>.TranslateResponse(System.Xml.XmlReader, System.Xml.XmlWriter)') | Translates a response [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message')-derived message's body, whose content is given by [reader](CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(XmlReader,XmlWriter).md#Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(System.Xml.XmlReader,System.Xml.XmlWriter).reader 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator<TRequestTransform,TResponseTransform>.TranslateResponse(System.Xml.XmlReader, System.Xml.XmlWriter).reader'), and outputs the results to [writer](CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(XmlReader,XmlWriter).md#Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(System.Xml.XmlReader,System.Xml.XmlWriter).writer 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator<TRequestTransform,TResponseTransform>.TranslateResponse(System.Xml.XmlReader, System.Xml.XmlWriter).writer'). |
