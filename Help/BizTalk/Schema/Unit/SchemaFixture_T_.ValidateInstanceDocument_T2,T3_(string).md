#### [Be.Stateless.BizTalk.Schema.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Schema](Be.Stateless.BizTalk.Unit.Schema.md 'Be.Stateless.BizTalk.Unit.Schema').[SchemaFixture&lt;T&gt;](SchemaFixture_T_.md 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>')

## SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(string) Method

Loads and validates an XML file against the [T](SchemaFixture_T_.md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.T 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.T'), [T2](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string).T2 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(string).T2') and [T3](SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string).md#Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string).T3 'Be.Stateless.BizTalk.Unit.Schema.SchemaFixture<T>.ValidateInstanceDocument<T2,T3>(string).T3') BizTalk Server schemas.

```csharp
protected System.Xml.XmlDocument ValidateInstanceDocument<T2,T3>(string filepath)
    where T2 : Microsoft.XLANGs.BaseTypes.SchemaBase, new()
    where T3 : Microsoft.XLANGs.BaseTypes.SchemaBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string).T2'></a>

`T2`

A supplementary type of the BizTalk Server schema to validate against.

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string).T3'></a>

`T3`

A supplementary type of the BizTalk Server schema to validate against.
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Schema.SchemaFixture_T_.ValidateInstanceDocument_T2,T3_(string).filepath'></a>

`filepath` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The path of the XML file to load and validate.

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
An [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') that has loaded and validated the content of the XML file.