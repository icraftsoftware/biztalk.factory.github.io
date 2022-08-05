#### [Be.Stateless.BizTalk.Schema.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Schema](Be.Stateless.BizTalk.Unit.Schema.md 'Be.Stateless.BizTalk.Unit.Schema')

## SchemaFixture<T> Class

This base class provides utility methods to validate XML instance documents against a BizTalk Server [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived schema.

```csharp
public abstract class SchemaFixture<T>
    where T : Microsoft.XLANGs.BaseTypes.SchemaBase, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T'></a>

`T`

The type of the BizTalk Server schema to validate against.

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; SchemaFixture<T>

| Methods | |
| :--- | :--- |
| [ValidateInstanceDocument(string, XmlSchemaContentProcessing)](SchemaFixture_T_.ValidateInstanceDocument(string,XmlSchemaContentProcessing).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument(string, System.Xml.Schema.XmlSchemaContentProcessing)') | Loads and validates an XML file against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') BizTalk Server schema. |
| [ValidateInstanceDocument(string)](SchemaFixture_T_.ValidateInstanceDocument(string).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument(string)') | Loads and validates an XML file against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') BizTalk Server schema. |
| [ValidateInstanceDocument(Stream, XmlSchemaContentProcessing)](SchemaFixture_T_.ValidateInstanceDocument(Stream,XmlSchemaContentProcessing).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument(System.IO.Stream, System.Xml.Schema.XmlSchemaContentProcessing)') | Validates an [Be.Stateless.BizTalk.Stream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream 'Be.Stateless.BizTalk.Stream') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') BizTalk Server schema. |
| [ValidateInstanceDocument(Stream)](SchemaFixture_T_.ValidateInstanceDocument(Stream).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument(System.IO.Stream)') | Validates an [Be.Stateless.BizTalk.Stream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream 'Be.Stateless.BizTalk.Stream') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') BizTalk Server schema. |
| [ValidateInstanceDocument(XmlDocument, XmlSchemaContentProcessing)](SchemaFixture_T_.ValidateInstanceDocument(XmlDocument,XmlSchemaContentProcessing).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument(System.Xml.XmlDocument, System.Xml.Schema.XmlSchemaContentProcessing)') | Validates an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') BizTalk Server schema. |
| [ValidateInstanceDocument(XmlDocument)](SchemaFixture_T_.ValidateInstanceDocument(XmlDocument).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument(System.Xml.XmlDocument)') | Validates an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') BizTalk Server schema. |
| [ValidateInstanceDocument(XmlReader, XmlSchemaContentProcessing)](SchemaFixture_T_.ValidateInstanceDocument(XmlReader,XmlSchemaContentProcessing).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument(System.Xml.XmlReader, System.Xml.Schema.XmlSchemaContentProcessing)') | Validates an [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') BizTalk Server schema. |
| [ValidateInstanceDocument(XmlReader)](SchemaFixture_T_.ValidateInstanceDocument(XmlReader).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument(System.Xml.XmlReader)') | Validates an [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') BizTalk Server schema. |
| [ValidateInstanceDocument&lt;T2,T3&gt;(string, XmlSchemaContentProcessing)](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string,XmlSchemaContentProcessing).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(string, System.Xml.Schema.XmlSchemaContentProcessing)') | Loads and validates an XML file against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T'), [T2](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string,XmlSchemaContentProcessing).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string,System.Xml.Schema.XmlSchemaContentProcessing).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(string, System.Xml.Schema.XmlSchemaContentProcessing).T2') and [T3](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string,XmlSchemaContentProcessing).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string,System.Xml.Schema.XmlSchemaContentProcessing).T3 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(string, System.Xml.Schema.XmlSchemaContentProcessing).T3') BizTalk Server schemas. |
| [ValidateInstanceDocument&lt;T2,T3&gt;(string)](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(string)') | Loads and validates an XML file against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T'), [T2](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(string).T2') and [T3](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string).T3 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(string).T3') BizTalk Server schemas. |
| [ValidateInstanceDocument&lt;T2,T3&gt;(Stream, XmlSchemaContentProcessing)](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(Stream,XmlSchemaContentProcessing).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.IO.Stream, System.Xml.Schema.XmlSchemaContentProcessing)') | Validates an [Be.Stateless.BizTalk.Stream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream 'Be.Stateless.BizTalk.Stream') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T'), [T2](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(Stream,XmlSchemaContentProcessing).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.IO.Stream,System.Xml.Schema.XmlSchemaContentProcessing).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.IO.Stream, System.Xml.Schema.XmlSchemaContentProcessing).T2') and [T3](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(Stream,XmlSchemaContentProcessing).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.IO.Stream,System.Xml.Schema.XmlSchemaContentProcessing).T3 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.IO.Stream, System.Xml.Schema.XmlSchemaContentProcessing).T3') BizTalk Server schemas. |
| [ValidateInstanceDocument&lt;T2,T3&gt;(Stream)](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(Stream).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.IO.Stream)') | Validates an [Be.Stateless.BizTalk.Stream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream 'Be.Stateless.BizTalk.Stream') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T'), [T2](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(Stream).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.IO.Stream).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.IO.Stream).T2') and [T3](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(Stream).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.IO.Stream).T3 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.IO.Stream).T3') BizTalk Server schemas. |
| [ValidateInstanceDocument&lt;T2,T3&gt;(XmlDocument, XmlSchemaContentProcessing)](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(XmlDocument,XmlSchemaContentProcessing).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.Xml.XmlDocument, System.Xml.Schema.XmlSchemaContentProcessing)') | Validates an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T'), [T2](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(XmlDocument,XmlSchemaContentProcessing).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.Xml.XmlDocument,System.Xml.Schema.XmlSchemaContentProcessing).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.Xml.XmlDocument, System.Xml.Schema.XmlSchemaContentProcessing).T2') and [T3](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(XmlDocument,XmlSchemaContentProcessing).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.Xml.XmlDocument,System.Xml.Schema.XmlSchemaContentProcessing).T3 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.Xml.XmlDocument, System.Xml.Schema.XmlSchemaContentProcessing).T3') BizTalk Server schemas. |
| [ValidateInstanceDocument&lt;T2,T3&gt;(XmlDocument)](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(XmlDocument).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.Xml.XmlDocument)') | Validates an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T'), [T2](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(XmlDocument).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.Xml.XmlDocument).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.Xml.XmlDocument).T2') and [T3](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(XmlDocument).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.Xml.XmlDocument).T3 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.Xml.XmlDocument).T3') BizTalk Server schemas. |
| [ValidateInstanceDocument&lt;T2,T3&gt;(XmlReader, XmlSchemaContentProcessing)](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(XmlReader,XmlSchemaContentProcessing).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.Xml.XmlReader, System.Xml.Schema.XmlSchemaContentProcessing)') | Validates an [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T'), [T2](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(XmlReader,XmlSchemaContentProcessing).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.Xml.XmlReader,System.Xml.Schema.XmlSchemaContentProcessing).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.Xml.XmlReader, System.Xml.Schema.XmlSchemaContentProcessing).T2') and [T3](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(XmlReader,XmlSchemaContentProcessing).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.Xml.XmlReader,System.Xml.Schema.XmlSchemaContentProcessing).T3 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.Xml.XmlReader, System.Xml.Schema.XmlSchemaContentProcessing).T3') BizTalk Server schemas. |
| [ValidateInstanceDocument&lt;T2,T3&gt;(XmlReader)](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(XmlReader).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.Xml.XmlReader)') | Validates an [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T'), [T2](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(XmlReader).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.Xml.XmlReader).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.Xml.XmlReader).T2') and [T3](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(XmlReader).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.Xml.XmlReader).T3 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.Xml.XmlReader).T3') BizTalk Server schemas. |
| [ValidateInstanceDocument&lt;T2&gt;(string, XmlSchemaContentProcessing)](SchemaFixture_T_.ValidateInstanceDocument_T2_(string,XmlSchemaContentProcessing).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(string, System.Xml.Schema.XmlSchemaContentProcessing)') | Loads and validates an XML file against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') and [T2](SchemaFixture_T_.ValidateInstanceDocument_T2_(string,XmlSchemaContentProcessing).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2_(string,System.Xml.Schema.XmlSchemaContentProcessing).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(string, System.Xml.Schema.XmlSchemaContentProcessing).T2') BizTalk Server schemas. |
| [ValidateInstanceDocument&lt;T2&gt;(string)](SchemaFixture_T_.ValidateInstanceDocument_T2_(string).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(string)') | Loads and validates an XML file against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') and [T2](SchemaFixture_T_.ValidateInstanceDocument_T2_(string).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2_(string).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(string).T2') BizTalk Server schemas. |
| [ValidateInstanceDocument&lt;T2&gt;(Stream, XmlSchemaContentProcessing)](SchemaFixture_T_.ValidateInstanceDocument_T2_(Stream,XmlSchemaContentProcessing).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(System.IO.Stream, System.Xml.Schema.XmlSchemaContentProcessing)') | Validates an [Be.Stateless.BizTalk.Stream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream 'Be.Stateless.BizTalk.Stream') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') and [T2](SchemaFixture_T_.ValidateInstanceDocument_T2_(Stream,XmlSchemaContentProcessing).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2_(System.IO.Stream,System.Xml.Schema.XmlSchemaContentProcessing).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(System.IO.Stream, System.Xml.Schema.XmlSchemaContentProcessing).T2') BizTalk Server schemas. |
| [ValidateInstanceDocument&lt;T2&gt;(Stream)](SchemaFixture_T_.ValidateInstanceDocument_T2_(Stream).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(System.IO.Stream)') | Validates an [Be.Stateless.BizTalk.Stream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream 'Be.Stateless.BizTalk.Stream') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') and [T2](SchemaFixture_T_.ValidateInstanceDocument_T2_(Stream).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2_(System.IO.Stream).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(System.IO.Stream).T2') BizTalk Server schemas. |
| [ValidateInstanceDocument&lt;T2&gt;(XmlDocument, XmlSchemaContentProcessing)](SchemaFixture_T_.ValidateInstanceDocument_T2_(XmlDocument,XmlSchemaContentProcessing).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(System.Xml.XmlDocument, System.Xml.Schema.XmlSchemaContentProcessing)') | Validates an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') and [T2](SchemaFixture_T_.ValidateInstanceDocument_T2_(XmlDocument,XmlSchemaContentProcessing).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2_(System.Xml.XmlDocument,System.Xml.Schema.XmlSchemaContentProcessing).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(System.Xml.XmlDocument, System.Xml.Schema.XmlSchemaContentProcessing).T2') BizTalk Server schemas. |
| [ValidateInstanceDocument&lt;T2&gt;(XmlDocument)](SchemaFixture_T_.ValidateInstanceDocument_T2_(XmlDocument).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(System.Xml.XmlDocument)') | Validates an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') and [T2](SchemaFixture_T_.ValidateInstanceDocument_T2_(XmlDocument).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2_(System.Xml.XmlDocument).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(System.Xml.XmlDocument).T2') BizTalk Server schemas. |
| [ValidateInstanceDocument&lt;T2&gt;(XmlReader, XmlSchemaContentProcessing)](SchemaFixture_T_.ValidateInstanceDocument_T2_(XmlReader,XmlSchemaContentProcessing).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(System.Xml.XmlReader, System.Xml.Schema.XmlSchemaContentProcessing)') | Validates an [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') and [T2](SchemaFixture_T_.ValidateInstanceDocument_T2_(XmlReader,XmlSchemaContentProcessing).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2_(System.Xml.XmlReader,System.Xml.Schema.XmlSchemaContentProcessing).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(System.Xml.XmlReader, System.Xml.Schema.XmlSchemaContentProcessing).T2') BizTalk Server schemas. |
| [ValidateInstanceDocument&lt;T2&gt;(XmlReader)](SchemaFixture_T_.ValidateInstanceDocument_T2_(XmlReader).md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(System.Xml.XmlReader)') | Validates an [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') and [T2](SchemaFixture_T_.ValidateInstanceDocument_T2_(XmlReader).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2_(System.Xml.XmlReader).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(System.Xml.XmlReader).T2') BizTalk Server schemas. |