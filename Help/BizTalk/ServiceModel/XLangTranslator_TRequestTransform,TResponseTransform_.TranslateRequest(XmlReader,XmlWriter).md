#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Xsl](Be.Stateless.BizTalk.Xml.Xsl.md 'Be.Stateless.BizTalk.Xml.Xsl').[XLangTranslator&lt;TRequestTransform,TResponseTransform&gt;](XLangTranslator_TRequestTransform,TResponseTransform_.md 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>')

## XLangTranslator<TRequestTransform,TResponseTransform>.TranslateRequest(XmlReader, XmlWriter) Method

Translates a request [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-derived message's body, whose content is given by [reader](XLangTranslator_TRequestTransform,TResponseTransform_.TranslateRequest(XmlReader,XmlWriter).md#Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator_TRequestTransform,TResponseTransform_.TranslateRequest(System.Xml.XmlReader,System.Xml.XmlWriter).reader 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>.TranslateRequest(System.Xml.XmlReader, System.Xml.XmlWriter).reader'), and outputs the results to [writer](XLangTranslator_TRequestTransform,TResponseTransform_.TranslateRequest(XmlReader,XmlWriter).md#Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator_TRequestTransform,TResponseTransform_.TranslateRequest(System.Xml.XmlReader,System.Xml.XmlWriter).writer 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>.TranslateRequest(System.Xml.XmlReader, System.Xml.XmlWriter).writer').

```csharp
protected override void TranslateRequest(System.Xml.XmlReader reader, System.Xml.XmlWriter writer);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator_TRequestTransform,TResponseTransform_.TranslateRequest(System.Xml.XmlReader,System.Xml.XmlWriter).reader'></a>

`reader` [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')

The [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') containing the input document.

<a name='Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator_TRequestTransform,TResponseTransform_.TranslateRequest(System.Xml.XmlReader,System.Xml.XmlWriter).writer'></a>

`writer` [System.Xml.XmlWriter](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlWriter 'System.Xml.XmlWriter')

The [System.Xml.XmlWriter](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlWriter 'System.Xml.XmlWriter') that will contain the output of the transform.

### Remarks
This override reuses the extension objects that have been defined inside the [TRequestTransform](XLangTranslator_TRequestTransform,TResponseTransform_.md#Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator_TRequestTransform,TResponseTransform_.TRequestTransform 'Be.Stateless.BizTalk.Xml.Xsl.XLangTranslator<TRequestTransform,TResponseTransform>.TRequestTransform').