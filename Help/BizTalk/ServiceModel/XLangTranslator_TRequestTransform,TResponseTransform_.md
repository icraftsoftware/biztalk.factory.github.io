#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Xsl](Be.Stateless.BizTalk.Xml.Xsl.md 'Be.Stateless.BizTalk.Xml.Xsl')

## XLangTranslator<TRequestTransform,TResponseTransform> Class

Translates [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')s back and forth to native generic WCF [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')s by applying an [Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase')-derived type XSLT transform to
their payloads.

```csharp
public class XLangTranslator<TRequestTransform,TResponseTransform> : Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase
    where TRequestTransform : Microsoft.XLANGs.BaseTypes.TransformBase, new()
    where TResponseTransform : Microsoft.XLANGs.BaseTypes.TransformBase, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator_TRequestTransform,TResponseTransform_.TRequestTransform'></a>

`TRequestTransform`

<a name='Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator_TRequestTransform,TResponseTransform_.TResponseTransform'></a>

`TResponseTransform`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [XsltTranslatorBase](XsltTranslatorBase.md 'Be.Stateless.BizTalk.Xml.Xsl.XsltTranslatorBase') &#129106; XLangTranslator<TRequestTransform,TResponseTransform>

Derived  
&#8627; [CompositeXLangTranslator&lt;TRequestTransform,TResponseTransform&gt;](CompositeXLangTranslator_TRequestTransform,TResponseTransform_.md 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXLangTranslator<TRequestTransform,TResponseTransform>')

| Properties | |
| :--- | :--- |
| [RequestXslt](XLangTranslator_TRequestTransform,TResponseTransform_.RequestXslt.md 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>.RequestXslt') | [System.Xml.Xsl.XslCompiledTransform](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XslCompiledTransform 'System.Xml.Xsl.XslCompiledTransform') to apply to the request [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')'s body. |
| [RequestXsltArguments](XLangTranslator_TRequestTransform,TResponseTransform_.RequestXsltArguments.md 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>.RequestXsltArguments') | The extension objects that have been defined inside the [TRequestTransform](XLangTranslator_TRequestTransform,TResponseTransform_.md#Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator_TRequestTransform,TResponseTransform_.TRequestTransform 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>.TRequestTransform'). |
| [ResponseXslt](XLangTranslator_TRequestTransform,TResponseTransform_.ResponseXslt.md 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>.ResponseXslt') | [System.Xml.Xsl.XslCompiledTransform](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XslCompiledTransform 'System.Xml.Xsl.XslCompiledTransform') to apply to get the response [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')'s body. |
| [ResponseXsltArguments](XLangTranslator_TRequestTransform,TResponseTransform_.ResponseXsltArguments.md 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>.ResponseXsltArguments') | The extension objects that have been defined inside the [TResponseTransform](XLangTranslator_TRequestTransform,TResponseTransform_.md#Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator_TRequestTransform,TResponseTransform_.TResponseTransform 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>.TResponseTransform'). |

| Methods | |
| :--- | :--- |
| [TranslateRequest(XmlReader, XmlWriter)](XLangTranslator_TRequestTransform,TResponseTransform_.TranslateRequest(XmlReader,XmlWriter).md 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>.TranslateRequest(System.Xml.XmlReader, System.Xml.XmlWriter)') | Translates a request [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-derived message's body, whose content is given by [reader](XLangTranslator_TRequestTransform,TResponseTransform_.TranslateRequest(XmlReader,XmlWriter).md#Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator_TRequestTransform,TResponseTransform_.TranslateRequest(System.Xml.XmlReader,System.Xml.XmlWriter).reader 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>.TranslateRequest(System.Xml.XmlReader, System.Xml.XmlWriter).reader'), and outputs the results to [writer](XLangTranslator_TRequestTransform,TResponseTransform_.TranslateRequest(XmlReader,XmlWriter).md#Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator_TRequestTransform,TResponseTransform_.TranslateRequest(System.Xml.XmlReader,System.Xml.XmlWriter).writer 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>.TranslateRequest(System.Xml.XmlReader, System.Xml.XmlWriter).writer'). |
| [TranslateResponse(XmlReader, XmlWriter)](XLangTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(XmlReader,XmlWriter).md 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>.TranslateResponse(System.Xml.XmlReader, System.Xml.XmlWriter)') | Translates a response [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')-derived message's body, whose content is given by [reader](XLangTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(XmlReader,XmlWriter).md#Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(System.Xml.XmlReader,System.Xml.XmlWriter).reader 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>.TranslateResponse(System.Xml.XmlReader, System.Xml.XmlWriter).reader'), and outputs the results to [writer](XLangTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(XmlReader,XmlWriter).md#Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(System.Xml.XmlReader,System.Xml.XmlWriter).writer 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>.TranslateResponse(System.Xml.XmlReader, System.Xml.XmlWriter).writer'). |
