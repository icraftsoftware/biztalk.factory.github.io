#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Xsl](Be.Stateless.BizTalk.Xml.Xsl.md 'Be.Stateless.BizTalk.Xml.Xsl')

## CompositeXLangTranslator<TRequestTransform,TResponseTransform> Class

Translates [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')s back and forth to native generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message')s by applying an [Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase')-derived type XSLT transform to their payloads.

```csharp
public class CompositeXLangTranslator<TRequestTransform,TResponseTransform> : Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform, TResponseTransform>
    where TRequestTransform : Microsoft.XLANGs.BaseTypes.TransformBase, new()
    where TResponseTransform : Microsoft.XLANGs.BaseTypes.TransformBase, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Xml.Xsl.CompositeXLangTranslator_TRequestTransform,TResponseTransform_.TRequestTransform'></a>

`TRequestTransform`

<a name='Be.Stateless.BizTalk.Xml.Xsl.CompositeXLangTranslator_TRequestTransform,TResponseTransform_.TResponseTransform'></a>

`TResponseTransform`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [XsltTranslatorBase](XsltTranslatorBase.md 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase') &#129106; [Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator&lt;](XLangTranslator_TRequestTransform,TResponseTransform_.md 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>')[TRequestTransform](CompositeXLangTranslator_TRequestTransform,TResponseTransform_.md#Be.Stateless.BizTalk.Xml.Xsl.CompositeXLangTranslator_TRequestTransform,TResponseTransform_.TRequestTransform 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXLangTranslator<TRequestTransform,TResponseTransform>.TRequestTransform')[,](XLangTranslator_TRequestTransform,TResponseTransform_.md 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>')[TResponseTransform](CompositeXLangTranslator_TRequestTransform,TResponseTransform_.md#Be.Stateless.BizTalk.Xml.Xsl.CompositeXLangTranslator_TRequestTransform,TResponseTransform_.TResponseTransform 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXLangTranslator<TRequestTransform,TResponseTransform>.TResponseTransform')[&gt;](XLangTranslator_TRequestTransform,TResponseTransform_.md 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>') &#129106; CompositeXLangTranslator<TRequestTransform,TResponseTransform>

| Methods | |
| :--- | :--- |
| [CreateMessageRequestFromXmlRequest&lt;TRequest&gt;(TRequest)](CompositeXLangTranslator_TRequestTransform,TResponseTransform_.CreateMessageRequestFromXmlRequest_TRequest_(TRequest).md 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXLangTranslator<TRequestTransform,TResponseTransform>.CreateMessageRequestFromXmlRequest<TRequest>(TRequest)') | Translates an [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') to a generic WCF [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message'). |
| [TranslateResponse(XmlReader, XmlWriter)](CompositeXLangTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(XmlReader,XmlWriter).md 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXLangTranslator<TRequestTransform,TResponseTransform>.TranslateResponse(System.Xml.XmlReader, System.Xml.XmlWriter)') | Translates a response [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message')-derived message's body, whose content is given by [reader](CompositeXLangTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(XmlReader,XmlWriter).md#Be.Stateless.BizTalk.Xml.Xsl.CompositeXLangTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(System.Xml.XmlReader,System.Xml.XmlWriter).reader 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXLangTranslator<TRequestTransform,TResponseTransform>.TranslateResponse(System.Xml.XmlReader, System.Xml.XmlWriter).reader'), and outputs the results to [writer](CompositeXLangTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(XmlReader,XmlWriter).md#Be.Stateless.BizTalk.Xml.Xsl.CompositeXLangTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(System.Xml.XmlReader,System.Xml.XmlWriter).writer 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXLangTranslator<TRequestTransform,TResponseTransform>.TranslateResponse(System.Xml.XmlReader, System.Xml.XmlWriter).writer'). |
