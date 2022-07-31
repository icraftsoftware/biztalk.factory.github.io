#### [Be.Stateless.BizTalk.Schema.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Schema](Be.Stateless.BizTalk.Unit.Schema.md 'Be.Stateless.BizTalk.Unit.Schema').[SchemaFixture&lt;T&gt;](SchemaFixture_T_.md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>')

## SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(XmlDocument, XmlSchemaContentProcessing) Method

Validates an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T'), [T2](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(XmlDocument,XmlSchemaContentProcessing).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.Xml.XmlDocument,System.Xml.Schema.XmlSchemaContentProcessing).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.Xml.XmlDocument, System.Xml.Schema.XmlSchemaContentProcessing).T2') and
[T3](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(XmlDocument,XmlSchemaContentProcessing).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.Xml.XmlDocument,System.Xml.Schema.XmlSchemaContentProcessing).T3 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(System.Xml.XmlDocument, System.Xml.Schema.XmlSchemaContentProcessing).T3') BizTalk Server schemas.

```csharp
protected System.Xml.XmlDocument ValidateInstanceDocument<T2,T3>(System.Xml.XmlDocument document, System.Xml.Schema.XmlSchemaContentProcessing contentProcessing)
    where T2 : Microsoft.XLANGs.BaseTypes.SchemaBase, new()
    where T3 : Microsoft.XLANGs.BaseTypes.SchemaBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.Xml.XmlDocument,System.Xml.Schema.XmlSchemaContentProcessing).T2'></a>

`T2`

A supplementary type of the BizTalk Server schema to validate against.

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.Xml.XmlDocument,System.Xml.Schema.XmlSchemaContentProcessing).T3'></a>

`T3`

A supplementary type of the BizTalk Server schema to validate against.
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.Xml.XmlDocument,System.Xml.Schema.XmlSchemaContentProcessing).document'></a>

`document` [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')

The [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') to validate.

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(System.Xml.XmlDocument,System.Xml.Schema.XmlSchemaContentProcessing).contentProcessing'></a>

`contentProcessing` [System.Xml.Schema.XmlSchemaContentProcessing](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaContentProcessing 'System.Xml.Schema.XmlSchemaContentProcessing')

Validation mode.

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
An [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') that has loaded and validated the content of the input [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument').