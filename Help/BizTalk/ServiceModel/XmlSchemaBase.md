#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Schema](Be.Stateless.BizTalk.Xml.Schema.md 'Be.Stateless.BizTalk.Xml.Schema')

## XmlSchemaBase Class

Base class that loads the content of an [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') from the [XmlSchemaBase](XmlSchemaBase.md 'Be.Stateless.BizTalk.Xml.Schema.XmlSchemaBase')-derived type's
assembly resources.

```csharp
public abstract class XmlSchemaBase :
Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; XmlSchemaBase

Implements [IXmlSchemaProvider](IXmlSchemaProvider.md 'Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider')

| Properties | |
| :--- | :--- |
| [Schema](XmlSchemaBase.Schema.md 'Be.Stateless.BizTalk.Xml.Schema.XmlSchemaBase.Schema') | The [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') against which to validate its XML representation. |

| Methods | |
| :--- | :--- |
| [ProvideSchema(XmlSchemaSet)](XmlSchemaBase.ProvideSchema(XmlSchemaSet).md 'Be.Stateless.BizTalk.Xml.Schema.XmlSchemaBase.ProvideSchema(System.Xml.Schema.XmlSchemaSet)') | Provides the [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') to the [schemaSet](XmlSchemaBase.ProvideSchema(XmlSchemaSet).md#Be.Stateless.BizTalk.Xml.Schema.XmlSchemaBase.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet 'Be.Stateless.BizTalk.Xml.Schema.XmlSchemaBase.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet') and the [System.Xml.Schema.XmlSchemaType](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaType 'System.Xml.Schema.XmlSchemaType') that controls the serialization of the type. |
