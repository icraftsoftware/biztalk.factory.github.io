#### [Be.Stateless.BizTalk.Schema.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Schema](Be.Stateless.BizTalk.Unit.Schema.md 'Be.Stateless.BizTalk.Unit.Schema').[SchemaFixture&lt;T&gt;](SchemaFixture_T_.md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>')

## SchemaFixture<T>.ValidateInstanceDocument(XmlReader, XmlSchemaContentProcessing) Method

Validates an [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') BizTalk Server schema.

```csharp
protected System.Xml.XmlDocument ValidateInstanceDocument(System.Xml.XmlReader reader, System.Xml.Schema.XmlSchemaContentProcessing contentProcessing);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument(System.Xml.XmlReader,System.Xml.Schema.XmlSchemaContentProcessing).reader'></a>

`reader` [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')

The [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') to validate.

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument(System.Xml.XmlReader,System.Xml.Schema.XmlSchemaContentProcessing).contentProcessing'></a>

`contentProcessing` [System.Xml.Schema.XmlSchemaContentProcessing](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaContentProcessing 'System.Xml.Schema.XmlSchemaContentProcessing')

Validation mode.

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
An [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') that has loaded and validated the content of the [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader').