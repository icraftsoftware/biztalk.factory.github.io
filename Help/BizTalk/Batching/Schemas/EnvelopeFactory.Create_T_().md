#### [Be.Stateless.BizTalk.Batching.Schemas](README.md 'README')
### [Be.Stateless.BizTalk.Message](Be.Stateless.BizTalk.Message.md 'Be.Stateless.BizTalk.Message').[EnvelopeFactory](EnvelopeFactory.md 'Be.Stateless.BizTalk.Message.EnvelopeFactory')

## EnvelopeFactory.Create<T>() Method

Creates an envelope template document for a given [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived envelope schema type [T](EnvelopeFactory.Create_T_().md#Be.Stateless.BizTalk.Message.EnvelopeFactory.Create_T_().T 'Be.Stateless.BizTalk.Message.EnvelopeFactory.Create<T>().T').

```csharp
public static System.Xml.XmlDocument Create<T>()
    where T : Microsoft.XLANGs.BaseTypes.SchemaBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Message.EnvelopeFactory.Create_T_().T'></a>

`T`

The [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived envelope schema type.

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
The envelope template document as an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument').

### Remarks
Notice the that the `<ns:parts-here xmlns:ns="urn:schemas.stateless.be:biztalk:batch:2012:12"/>` XML
placeholder element will be inserted where the content of the envelope's body must be located; this provides an easy
way for XSLT maps to latter insert the envelope's body content by overriding this placeholder.