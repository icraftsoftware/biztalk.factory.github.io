#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Schema](Be.Stateless.BizTalk.Schema.md 'Be.Stateless.BizTalk.Schema')

## ISchemaAnnotationCollection Interface

Provides access to annotations embedded in [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived schema definitions.

```csharp
public interface ISchemaAnnotationCollection
```

Derived  
&#8627; [SchemaAnnotationCollection](SchemaAnnotationCollection.md 'Be.Stateless.BizTalk.Schema.SchemaAnnotationCollection')

### Example
The following example illustrates how to embed BizTalk Factory annotations. Note that other annotations specific to
Microsoft BizTalk Server might coexist but are not illustrated.

```csharp
<xs:schema targetNamespace='urn:schemas.stateless.be:biztalk:tests:annotated:2013:01'
           xmlns:san='urn:schemas.stateless.be:biztalk:annotations:2013:01'
           xmlns:xs='http://www.w3.org/2001/XMLSchema'>
  <xs:element name='Root'>
    <xs:annotation>
      <xs:appinfo>
        ...
        <san:EnvelopeMapSpecName>Be.Stateless.BizTalk.Transform.Identity, Be.Stateless.BizTalk.Transform, Version=1.0.0.0, Culture=neutral, PublicKeyToken=3707daa0b119fc14</san:EnvelopeMapSpecName>
        <san:Properties xmlns:tp='urn:schemas.stateless.be:biztalk:properties:tracking:2012:04'>
          <tp:Value1 xpath="/*[local-name()='Root']/*[local-name()='Message']/*[local-name()='Id']"/>
        </san:Properties>
        ...
      </xs:appinfo>
    </xs:annotation>
    <xs:complexType/>
  </xs:element>
</xs:schema>
```

### Remarks

Only annotations declared in the schema annotation namespace defined by BizTalk Factory, i.e.
`urn:schemas.stateless.be:biztalk:annotations:2013:01` are considered; all other annotations are ignored.

Notice that there is no transitive discovery of the annotations across the XSD type definitions and that only annotations
embedded directly underneath the root node of the relevant [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived schema are loaded.

| Methods | |
| :--- | :--- |
| [Find&lt;T&gt;()](ISchemaAnnotationCollection.Find_T_().md 'Be.Stateless.BizTalk.Schema.ISchemaAnnotationCollection.Find<T>()') | Look up for an embedded schema annotation of type [T](ISchemaAnnotationCollection.Find_T_().md#Be.Stateless.BizTalk.Schema.ISchemaAnnotationCollection.Find_T_().T 'Be.Stateless.BizTalk.Schema.ISchemaAnnotationCollection.Find<T>().T'). |
