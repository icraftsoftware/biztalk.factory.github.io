#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[ValidatingXmlReader](ValidatingXmlReader.md 'Be.Stateless.Xml.ValidatingXmlReader')

## ValidatingXmlReader.Create<T>(Stream, XmlSchemaContentProcessing) Method

```csharp
public static System.Xml.XmlReader Create<T>(System.IO.Stream input, System.Xml.Schema.XmlSchemaContentProcessing contentProcessing=System.Xml.Schema.XmlSchemaContentProcessing.Strict)
    where T : System.Xml.Schema.XmlSchema, new();
```
#### Type parameters

<a name='Be.Stateless.Xml.ValidatingXmlReader.Create_T_(System.IO.Stream,System.Xml.Schema.XmlSchemaContentProcessing).T'></a>

`T`
#### Parameters

<a name='Be.Stateless.Xml.ValidatingXmlReader.Create_T_(System.IO.Stream,System.Xml.Schema.XmlSchemaContentProcessing).input'></a>

`input` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

<a name='Be.Stateless.Xml.ValidatingXmlReader.Create_T_(System.IO.Stream,System.Xml.Schema.XmlSchemaContentProcessing).contentProcessing'></a>

`contentProcessing` [System.Xml.Schema.XmlSchemaContentProcessing](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaContentProcessing 'System.Xml.Schema.XmlSchemaContentProcessing')

#### Returns
[System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')