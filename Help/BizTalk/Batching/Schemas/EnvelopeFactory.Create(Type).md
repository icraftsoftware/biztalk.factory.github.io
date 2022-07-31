#### [Be.Stateless.BizTalk.Batching.Schemas](README.md 'README')
### [Be.Stateless.BizTalk.Message](Be.Stateless.BizTalk.Message.md 'Be.Stateless.BizTalk.Message').[EnvelopeFactory](EnvelopeFactory.md 'Be.Stateless.BizTalk.Message.EnvelopeFactory')

## EnvelopeFactory.Create(Type) Method

Creates an envelope template document for a given [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived envelope schema type.

```csharp
public static System.Xml.XmlDocument Create(System.Type schema);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Message.EnvelopeFactory.Create(System.Type).schema'></a>

`schema` [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')

The [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived envelope schema type.

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
The envelope template document as an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument').

### Remarks
Notice the that the `<ns:parts-here xmlns:ns="urn:schemas.stateless.be:biztalk:batch:2012:12"/>` XML
placeholder element will be inserted where the content of the envelope's body must be located; this provides an easy
way for XSLT maps to latter insert the envelope's body content by overriding this placeholder.