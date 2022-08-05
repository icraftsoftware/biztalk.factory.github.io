#### [Be.Stateless.BizTalk.Batching](README.md 'README')
### [Be.Stateless.BizTalk.Schema](Be.Stateless.BizTalk.Schema.md 'Be.Stateless.BizTalk.Schema')

## EnvelopeMapAnnotation Class

Provides access to annotations embedded in [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived schema definitions.

```csharp
public class EnvelopeMapAnnotation :
Be.Stateless.BizTalk.Schema.ISchemaAnnotation<Be.Stateless.BizTalk.Schema.EnvelopeMapAnnotation>
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; EnvelopeMapAnnotation

Implements [Be.Stateless.BizTalk.Schema.ISchemaAnnotation&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schema.ISchemaAnnotation-1 'Be.Stateless.BizTalk.Schema.ISchemaAnnotation`1')[EnvelopeMapAnnotation](EnvelopeMapAnnotation.md 'Be.Stateless.BizTalk.Schema.EnvelopeMapAnnotation')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schema.ISchemaAnnotation-1 'Be.Stateless.BizTalk.Schema.ISchemaAnnotation`1')

### Example
The following example illustrates how to embed BizTalk Factory annotations. Note that there other annotations specific
to Microsoft BizTalk Server might coexist but are not illustrated.

```csharp
<xs:schema targetNamespace='urn:schemas.stateless.be:biztalk:tests:annotated:2013:01'
           xmlns:san='urn:schemas.stateless.be:biztalk:annotations:2013:01'
           xmlns:xs='http://www.w3.org/2001/XMLSchema'>
  <xs:element name='Root'>
    <xs:annotation>
      <xs:appinfo>
        ...
        <san:EnvelopeMapSpecName>
          Be.Stateless.BizTalk.Maps.ToXml.BatchContentToAnyEnvelope, Be.Stateless.BizTalk.Batching.Maps, Version=2.1.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14
        </san:EnvelopeMapSpecName>
        ...
      </xs:appinfo>
    </xs:annotation>
    <xs:complexType/>
  </xs:element>
</xs:schema>
```

### Remarks

Only annotations declared in the schema annotation namespace defined by BizTalk Factory, i.e.
`urn:schemas.stateless.be:biztalk:annotations:2013:01` are considered; all other annotations are discarded.

Notice that there is no transitive discovery of the annotations across the XSD type definitions and that only
annotations embedded directly underneath the root node of the relevant [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived schema are
loaded.

| Properties | |
| :--- | :--- |
| [EnvelopeMapType](EnvelopeMapAnnotation.EnvelopeMapType.md 'Be.Stateless.BizTalk.Schema.EnvelopeMapAnnotation.EnvelopeMapType') | The [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type') of the [Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase')-derived XSLT transform that has to be applied when transforming from a [Be.Stateless.BizTalk.Schemas.Xml.Batch.Content](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schemas.Xml.Batch.Content 'Be.Stateless.BizTalk.Schemas.Xml.Batch.Content') payload to the [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived envelope schema which embeds this annotation. |

| Methods | |
| :--- | :--- |
| [Build(ISchemaAnnotationReader)](EnvelopeMapAnnotation.Build(ISchemaAnnotationReader).md 'Be.Stateless.BizTalk.Schema.EnvelopeMapAnnotation.Build(Be.Stateless.BizTalk.Schema.ISchemaAnnotationReader)') | |
