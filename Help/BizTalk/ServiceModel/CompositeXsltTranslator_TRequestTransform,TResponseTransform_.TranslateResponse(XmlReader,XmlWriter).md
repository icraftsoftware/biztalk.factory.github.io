#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Xsl](Be.Stateless.BizTalk.Xml.Xsl.md 'Be.Stateless.BizTalk.Xml.Xsl').[CompositeXsltTranslator&lt;TRequestTransform,TResponseTransform&gt;](CompositeXsltTranslator_TRequestTransform,TResponseTransform_.md 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator<TRequestTransform,TResponseTransform>')

## CompositeXsltTranslator<TRequestTransform,TResponseTransform>.TranslateResponse(XmlReader, XmlWriter) Method

Translates a response [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message')-derived message's body, whose content is given by [reader](CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(XmlReader,XmlWriter).md#Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(System.Xml.XmlReader,System.Xml.XmlWriter).reader 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator<TRequestTransform,TResponseTransform>.TranslateResponse(System.Xml.XmlReader, System.Xml.XmlWriter).reader'), and outputs the results to [writer](CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(XmlReader,XmlWriter).md#Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(System.Xml.XmlReader,System.Xml.XmlWriter).writer 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator<TRequestTransform,TResponseTransform>.TranslateResponse(System.Xml.XmlReader, System.Xml.XmlWriter).writer').

```csharp
protected override void TranslateResponse(System.Xml.XmlReader reader, System.Xml.XmlWriter writer);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(System.Xml.XmlReader,System.Xml.XmlWriter).reader'></a>

`reader` [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')

The [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') containing the input document.

<a name='Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TranslateResponse(System.Xml.XmlReader,System.Xml.XmlWriter).writer'></a>

`writer` [System.Xml.XmlWriter](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlWriter 'System.Xml.XmlWriter')

The [System.Xml.XmlWriter](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlWriter 'System.Xml.XmlWriter') that will contain the output of the transform.

### Remarks
It wraps both the original [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')-derived request's [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') and the [Be.Stateless.BizTalk.Message](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Message 'Be.Stateless.BizTalk.Message') response's [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') in a [Be.Stateless.BizTalk.Xml.CompositeXmlReader](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Xml.CompositeXmlReader 'Be.Stateless.BizTalk.Xml.CompositeXmlReader') before applying the
[TResponseTransform](CompositeXsltTranslator_TRequestTransform,TResponseTransform_.md#Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator_TRequestTransform,TResponseTransform_.TResponseTransform 'Be.Stateless.BizTalk.Xml.Xsl.CompositeXsltTranslator<TRequestTransform,TResponseTransform>.TResponseTransform') transform.