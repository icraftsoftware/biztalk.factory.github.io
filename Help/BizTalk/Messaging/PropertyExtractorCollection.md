#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Schema.Annotation](Be.Stateless.BizTalk.Schema.Annotation.md 'Be.Stateless.BizTalk.Schema.Annotation')

## PropertyExtractorCollection Class

Collection of [PropertyExtractor](PropertyExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor')-derived extractors that supports back and forth serialization to
XML.

```csharp
public class PropertyExtractorCollection :
System.Collections.Generic.IEnumerable<Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor>,
System.Collections.IEnumerable,
System.Xml.Serialization.IXmlSerializable
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; PropertyExtractorCollection

Derived  
&#8627; [PropertyExtractorCollectionSerializerSurrogate](PropertyExtractorCollectionSerializerSurrogate.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionSerializerSurrogate')

Implements [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[PropertyExtractor](PropertyExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1'), [System.Collections.IEnumerable](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.IEnumerable 'System.Collections.IEnumerable'), [System.Xml.Serialization.IXmlSerializable](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.IXmlSerializable 'System.Xml.Serialization.IXmlSerializable')

### Remarks

The XML serialization format complies to the following XML pseudo-schema, specifically, its structure and
annotation namespace (`urn:schemas.stateless.be:biztalk:annotations:2013:01`):

```csharp
<san:Properties [extractorPrecedence='pipeline | pipelineOnly | schema | schemaOnly']
                xmlns:tp='urn:schemas.stateless.be:biztalk:properties:tracking:2012:04'
                xmlns:san='urn:schemas.stateless.be:biztalk:annotations:2013:01'>
  <tp:Value1 [mode="clear | ignore | promote | write"]
             [promoted="true"]
             value="constant-string-literal"/>
  <tp:Value2 [mode="clear | demote | ignore | promote | write"]
             [qnameValue="localName | name"]
             [promoted="true"]
             xpath="/*[local-name()='Send']/*[local-name()='Message']/*[local-name()='Subject']"/>
  <tp:Value3 mode="clear | ignore"/>
</san:Properties>
```

Notice that the '`promoted`' attribute is being supported for backward compatibility but its usage is
deprecated in favor of the '`mode`' attribute.

| Constructors | |
| :--- | :--- |
| [PropertyExtractorCollection()](PropertyExtractorCollection.PropertyExtractorCollection().md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.PropertyExtractorCollection()') | |
| [PropertyExtractorCollection(ExtractorPrecedence, PropertyExtractor[])](PropertyExtractorCollection.PropertyExtractorCollection(ExtractorPrecedence,PropertyExtractor[]).md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.PropertyExtractorCollection(Be.Stateless.BizTalk.Schema.Annotation.ExtractorPrecedence, Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor[])') | |
| [PropertyExtractorCollection(ExtractorPrecedence, IEnumerable&lt;PropertyExtractor&gt;)](PropertyExtractorCollection.PropertyExtractorCollection(ExtractorPrecedence,IEnumerable_PropertyExtractor_).md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.PropertyExtractorCollection(Be.Stateless.BizTalk.Schema.Annotation.ExtractorPrecedence, System.Collections.Generic.IEnumerable<Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor>)') | |
| [PropertyExtractorCollection(PropertyExtractor[])](PropertyExtractorCollection.PropertyExtractorCollection(PropertyExtractor[]).md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.PropertyExtractorCollection(Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor[])') | |
| [PropertyExtractorCollection(IEnumerable&lt;PropertyExtractor&gt;)](PropertyExtractorCollection.PropertyExtractorCollection(IEnumerable_PropertyExtractor_).md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.PropertyExtractorCollection(System.Collections.Generic.IEnumerable<Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor>)') | |

| Properties | |
| :--- | :--- |
| [Empty](PropertyExtractorCollection.Empty.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.Empty') | |
| [Precedence](PropertyExtractorCollection.Precedence.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.Precedence') | Precedence of the [PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') to be used should extractors declared by XML schema annotations be merged to extractors configured by the pipeline. |

| Methods | |
| :--- | :--- |
| [GetEnumerator()](PropertyExtractorCollection.GetEnumerator().md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.GetEnumerator()') | |
| [GetSchema()](PropertyExtractorCollection.GetSchema().md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.GetSchema()') | |
| [ReadXml(XmlReader)](PropertyExtractorCollection.ReadXml(XmlReader).md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.ReadXml(System.Xml.XmlReader)') | Deserializes the [Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.Extractors](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.Extractors 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.Extractors') state property from its XML serialization format. |
| [Union(PropertyExtractorCollection)](PropertyExtractorCollection.Union(PropertyExtractorCollection).md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.Union(Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection)') | Merges two sets of [PropertyExtractor](PropertyExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor')-derived extractors by honoring their [Precedence](PropertyExtractorCollection.Precedence.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.Precedence') and assuming that this [PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') instance contains the [PropertyExtractor](PropertyExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor')s configured by XML schema annotations and that [PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') being merged into contains the [PropertyExtractor](PropertyExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor')s configured by the pipeline. |
| [WriteXml(XmlWriter)](PropertyExtractorCollection.WriteXml(XmlWriter).md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.WriteXml(System.Xml.XmlWriter)') | Serializes the [Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.Extractors](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.Extractors 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.Extractors') state property to its XML serialization format. |

| Operators | |
| :--- | :--- |
| [implicit operator PropertyExtractorCollection(PropertyExtractor[])](PropertyExtractorCollection.implicitoperatorPropertyExtractorCollection(PropertyExtractor[]).md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.op_Implicit Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection(Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor[])') | |

| Explicit Interface Implementations | |
| :--- | :--- |
| [System.Collections.IEnumerable.GetEnumerator()](PropertyExtractorCollection.System.Collections.IEnumerable.GetEnumerator().md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.System.Collections.IEnumerable.GetEnumerator()') | |
