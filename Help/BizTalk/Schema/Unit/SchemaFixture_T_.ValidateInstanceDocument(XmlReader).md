#### [Be.Stateless.BizTalk.Schema.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Schema](Be.Stateless.BizTalk.Unit.Schema.md 'Be.Stateless.BizTalk.Unit.Schema').[SchemaFixture&lt;T&gt;](SchemaFixture_T_.md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>')

## SchemaFixture<T>.ValidateInstanceDocument(XmlReader) Method

Validates an [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') BizTalk Server schema.

```csharp
protected System.Xml.XmlDocument ValidateInstanceDocument(System.Xml.XmlReader reader);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument(System.Xml.XmlReader).reader'></a>

`reader` [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')

The [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') to validate.

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
An [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') that has loaded and validated the content of the [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader').