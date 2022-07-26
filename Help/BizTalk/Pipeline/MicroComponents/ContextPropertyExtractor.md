#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent')

## ContextPropertyExtractor Class

This component allows to manipulate the message context by either clearing, demoting, writing or promoting property
values. These values can either be constant or extracted out of an XML message by defining XPath expressions. Notice
that these XPath expressions are less restrictive than the traditional canonical XPath expressions supported by BizTalk
Server; limitations are however still present and relatively strong.

```csharp
public class ContextPropertyExtractor :
Be.Stateless.BizTalk.MicroComponent.IMicroComponent
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ContextPropertyExtractor

Implements [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')

### Example

Example of an XML fragment configuration that can either be declared at the pipeline-level configuration or directly
embedded in a schema, [Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection'): 

```csharp
<san:Properties [extractorPrecedence='pipeline | pipelineOnly | schema | schemaOnly']
                xmlns:tp='urn:schemas.stateless.be:biztalk:properties:tracking:2012:04'
                xmlns:san='urn:schemas.stateless.be:biztalk:annotations:2013:01'>
  <tp:Value1 [mode="clear | ignore | promote | write"]
             value="constant-string-literal"/>
  <tp:Value2 [mode="clear | demote | ignore | promote | write"]
             [qnameValue="localName | name"]
             xpath="/*[local-name()='Send']/*[local-name()='Message']/*[local-name()='Subject']"/>
  <tp:Value3 mode="clear | ignore"/>
</san:Properties>
```

Notice that the `san:extractorPrecedence` attribute is relevant only when configured at the pipeline level and can
only have one of the following values: `pipeline`, `pipelineOnly`, `schema`, or `schemaOnly`.

### Remarks

Most properties to promote or write should be configured directly in the message schemas, and not at the pipeline level
using this component's configuration. The same XML fragment used to configure these properties can be both embedded
directly as annotations in a schema or configured at the pipeline level.

The known limitations on the supported XPath expressions are:
- No namespace prefixes may be used in the XPath queries. If you need to match a specific namespace, a predicate in the
  form of `/*[local-name()='element' and namespace-uri()='urn']` must be used.
- Position predicates only work when expressed directly on an element name. Thus `/element[1]` works, but
  `/*[local-name()='element' and position()=1]` doesn't.
- Most XPath functions may not be used.

Internally, the component uses the [Microsoft.BizTalk.Streaming.XPathMutatorStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.XPathMutatorStream 'Microsoft.BizTalk.Streaming.XPathMutatorStream') from BizTalk, which itself uses the [Microsoft.BizTalk.XPath.XPathReader](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.XPath.XPathReader 'Microsoft.BizTalk.XPath.XPathReader'). The limitations thus come from these classes. For useful background information about the
implementation, the following resources may be consulted:
- [The BizTalk
            XPathMutatorStream: pros and cons](http://www.codit.eu/Blog/post/2010/01/22/The-BizTalk-XPathMutatorStream-pros-and-cons.aspx 'http://www.codit.eu/Blog/post/2010/01/22/The-BizTalk-XPathMutatorStream-pros-and-cons.aspx')
- [XpathMutatorStream: Great functionality
            for every BizTalk Developer.](http://bloggingabout.net/blogs/wellink/archive/2006/03/03/11207.aspx 'http://bloggingabout.net/blogs/wellink/archive/2006/03/03/11207.aspx')
- [XPathMutatorStream](http://martijnh.blogspot.com/2006/03/xpathmutatorstream.html 'http://martijnh.blogspot.com/2006/03/xpathmutatorstream.html')
- [
            Updating repeating nodes in an XML Document with the same value using XPathMutatorStream](http://connectedthoughts.wordpress.com/2008/05/31/updating-repeating-nodes-in-an-xml-document-with-the-same-value-using-xpathmutatorstream/ 'http://connectedthoughts.wordpress.com/2008/05/31/updating-repeating-nodes-in-an-xml-document-with-the-same-value-using-xpathmutatorstream/')
- [The Best of Both Worlds: Combining XPath with the XmlReader](http://msdn.microsoft.com/en-us/library/ms950778.aspx 'http://msdn.microsoft.com/en-us/library/ms950778.aspx')

If the configured XPath expressions lead to multiple matches in the message, only the first match value is taken into
account for extraction (i.e. write or promote) and other matches are discarded. The component can possibly be slightly
enhanced to take a specific match index into account, by modifying the [ReactiveXPathExtractorCollection.OnMatch](https://docs.microsoft.com/en-us/dotnet/api/ReactiveXPathExtractorCollection.OnMatch 'ReactiveXPathExtractorCollection.OnMatch') method. Given the
limitations of the component, it could be necessary to change its implementation in the future if it cannot meet the new
requirements that may arise. The current implementation uses a full streaming approach, and the alternate way to do it
is using an [System.Xml.XPath.XPathNavigator](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.XPathNavigator 'System.Xml.XPath.XPathNavigator') in combination with a [Microsoft.BizTalk.Streaming.VirtualStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.VirtualStream 'Microsoft.BizTalk.Streaming.VirtualStream'). That would
allow almost all XPath queries of arbitrary complexity, at the cost of some performance loss.

### See Also
- [Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection')
- [Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode 'Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode')
- [Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor')
- [Be.Stateless.BizTalk.Schema.Annotation.ConstantExtractor](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schema.Annotation.ConstantExtractor 'Be.Stateless.BizTalk.Schema.Annotation.ConstantExtractor')
- [Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor')

| Properties | |
| :--- | :--- |
| [Extractors](ContextPropertyExtractor.Extractors.md 'Be.Stateless.BizTalk.MicroComponent.ContextPropertyExtractor.Extractors') | |
| [ExtractorSerializerSurrogate](ContextPropertyExtractor.ExtractorSerializerSurrogate.md 'Be.Stateless.BizTalk.MicroComponent.ContextPropertyExtractor.ExtractorSerializerSurrogate') | |

| Methods | |
| :--- | :--- |
| [Execute(IPipelineContext, IBaseMessage)](ContextPropertyExtractor.Execute(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.MicroComponent.ContextPropertyExtractor.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
