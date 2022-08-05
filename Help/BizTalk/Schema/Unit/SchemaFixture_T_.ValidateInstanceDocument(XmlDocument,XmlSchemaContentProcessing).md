#### [Be.Stateless.BizTalk.Schema.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Schema](Be.Stateless.BizTalk.Unit.Schema.md 'Be.Stateless.BizTalk.Unit.Schema').[SchemaFixture&lt;T&gt;](SchemaFixture_T_.md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>')

## SchemaFixture<T>.ValidateInstanceDocument(XmlDocument, XmlSchemaContentProcessing) Method

Validates an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') BizTalk Server schema.

```csharp
protected System.Xml.XmlDocument ValidateInstanceDocument(System.Xml.XmlDocument document, System.Xml.Schema.XmlSchemaContentProcessing contentProcessing);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument(System.Xml.XmlDocument,System.Xml.Schema.XmlSchemaContentProcessing).document'></a>

`document` [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')

The [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') to validate.

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument(System.Xml.XmlDocument,System.Xml.Schema.XmlSchemaContentProcessing).contentProcessing'></a>

`contentProcessing` [System.Xml.Schema.XmlSchemaContentProcessing](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaContentProcessing 'System.Xml.Schema.XmlSchemaContentProcessing')

Validation mode.

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
An [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') that has loaded and validated the content of the input [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument').