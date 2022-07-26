#### [Be.Stateless.BizTalk.Xml](README.md 'README')
### [Be.Stateless.BizTalk.Xml](Be.Stateless.BizTalk.Xml.md 'Be.Stateless.BizTalk.Xml').[ValidatingXmlReader](ValidatingXmlReader.md 'Be.Stateless.BizTalk.Xml.ValidatingXmlReader')

## ValidatingXmlReader.Create<T1,T2>(Stream, XmlSchemaContentProcessing) Method

```csharp
public static System.Xml.XmlReader Create<T1,T2>(System.IO.Stream input, System.Xml.Schema.XmlSchemaContentProcessing contentProcessing=System.Xml.Schema.XmlSchemaContentProcessing.Strict)
    where T1 : Microsoft.XLANGs.BaseTypes.SchemaBase, new()
    where T2 : Microsoft.XLANGs.BaseTypes.SchemaBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Xml.ValidatingXmlReader.Create_T1,T2_(System.IO.Stream,System.Xml.Schema.XmlSchemaContentProcessing).T1'></a>

`T1`

<a name='Be.Stateless.BizTalk.Xml.ValidatingXmlReader.Create_T1,T2_(System.IO.Stream,System.Xml.Schema.XmlSchemaContentProcessing).T2'></a>

`T2`
#### Parameters

<a name='Be.Stateless.BizTalk.Xml.ValidatingXmlReader.Create_T1,T2_(System.IO.Stream,System.Xml.Schema.XmlSchemaContentProcessing).input'></a>

`input` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

<a name='Be.Stateless.BizTalk.Xml.ValidatingXmlReader.Create_T1,T2_(System.IO.Stream,System.Xml.Schema.XmlSchemaContentProcessing).contentProcessing'></a>

`contentProcessing` [System.Xml.Schema.XmlSchemaContentProcessing](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaContentProcessing 'System.Xml.Schema.XmlSchemaContentProcessing')

#### Returns
[System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')