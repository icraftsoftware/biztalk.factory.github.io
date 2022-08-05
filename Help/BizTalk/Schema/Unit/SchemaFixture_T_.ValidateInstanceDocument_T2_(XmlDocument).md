#### [Be.Stateless.BizTalk.Schema.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Schema](Be.Stateless.BizTalk.Unit.Schema.md 'Be.Stateless.BizTalk.Unit.Schema').[SchemaFixture&lt;T&gt;](SchemaFixture_T_.md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>')

## SchemaFixture<T>.ValidateInstanceDocument<T2>(XmlDocument) Method

Validates an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T') and [T2](SchemaFixture_T_.ValidateInstanceDocument_T2_(XmlDocument).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2_(System.Xml.XmlDocument).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2>(System.Xml.XmlDocument).T2') BizTalk
Server schemas.

```csharp
protected System.Xml.XmlDocument ValidateInstanceDocument<T2>(System.Xml.XmlDocument document)
    where T2 : Microsoft.XLANGs.BaseTypes.SchemaBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2_(System.Xml.XmlDocument).T2'></a>

`T2`

A supplementary type of the BizTalk Server schema to validate against.
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2_(System.Xml.XmlDocument).document'></a>

`document` [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')

The [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') to validate.

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
An [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') that has loaded and validated the content of the input [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument').