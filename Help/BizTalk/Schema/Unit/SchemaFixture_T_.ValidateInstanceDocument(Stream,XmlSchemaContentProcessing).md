#### [Be.Stateless.BizTalk.Schema.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Schema](Be.Stateless.BizTalk.Unit.Schema.md 'Be.Stateless.BizTalk.Unit.Schema').[SchemaFixture&lt;T&gt;](SchemaFixture_T_.md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>')

## SchemaFixture<T>.ValidateInstanceDocument(Stream, XmlSchemaContentProcessing) Method

Validates an [Be.Stateless.BizTalk.Stream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream 'Be.Stateless.BizTalk.Stream') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') BizTalk Server schema.

```csharp
protected System.Xml.XmlDocument ValidateInstanceDocument(System.IO.Stream stream, System.Xml.Schema.XmlSchemaContentProcessing contentProcessing);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument(System.IO.Stream,System.Xml.Schema.XmlSchemaContentProcessing).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The [Be.Stateless.BizTalk.Stream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream 'Be.Stateless.BizTalk.Stream') to validate.

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument(System.IO.Stream,System.Xml.Schema.XmlSchemaContentProcessing).contentProcessing'></a>

`contentProcessing` [System.Xml.Schema.XmlSchemaContentProcessing](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaContentProcessing 'System.Xml.Schema.XmlSchemaContentProcessing')

Validation mode.

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
An [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') that has loaded and validated the content of the XML [Be.Stateless.BizTalk.Stream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream 'Be.Stateless.BizTalk.Stream').