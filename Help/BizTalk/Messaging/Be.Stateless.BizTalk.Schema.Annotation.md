#### [Be.Stateless.BizTalk.Messaging](README.md 'README')

## Be.Stateless.BizTalk.Schema.Annotation Namespace

| Classes | |
| :--- | :--- |
| [ConstantExtractor](ConstantExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.ConstantExtractor') | |
| [PropertyExtractor](PropertyExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor') | |
| [PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') | Collection of [PropertyExtractor](PropertyExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor')-derived extractors that supports back and forth serialization to XML. |
| [PropertyExtractorCollectionConverter](PropertyExtractorCollectionConverter.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter') | Converts a [PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') back and forth to a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String'). |
| [PropertyExtractorCollectionSerializerSurrogate](PropertyExtractorCollectionSerializerSurrogate.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionSerializerSurrogate') | |
| [QNameValueExtractor](QNameValueExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor') | Denotes a context property whose only the local part of a QName value will be extracted from an [Microsoft.BizTalk.Message.Interop.IBaseMessagePart](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessagePart 'Microsoft.BizTalk.Message.Interop.IBaseMessagePart')'s payload while being processed by the `Be.Stateless.BizTalk.Component.ContextPropertyExtractorComponent` pipeline component. |
| [XPathExtractor](XPathExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor') | Denotes a context property whose value will be extracted from an [Microsoft.BizTalk.Message.Interop.IBaseMessagePart](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessagePart 'Microsoft.BizTalk.Message.Interop.IBaseMessagePart')'s payload while being processed by the `Be.Stateless.BizTalk.Component.ContextPropertyExtractorComponent` pipeline component. |

| Enums | |
| :--- | :--- |
| [ExtractionMode](ExtractionMode.md 'Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode') | Denotes how a context property has to be processed by the `Be.Stateless.BizTalk.Component.ContextPropertyExtractorComponent` pipeline component. |
| [ExtractorPrecedence](ExtractorPrecedence.md 'Be.Stateless.BizTalk.Schema.Annotation.ExtractorPrecedence') | Determines how to merge two [PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') instances. |
| [QNameValueExtractionMode](QNameValueExtractionMode.md 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractionMode') | Denotes how the value, which might be a QName, pointed to by an [QNameValueExtractor](QNameValueExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.QNameValueExtractor') is extracted. This is typically the case for the [System.Xml.Schema.XmlSchema.InstanceNamespace](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema.InstanceNamespace 'System.Xml.Schema.XmlSchema.InstanceNamespace') type attribute's value. |
