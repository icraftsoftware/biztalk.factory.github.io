#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels](Be.Stateless.BizTalk.ServiceModel.Channels.md 'Be.Stateless.BizTalk.ServiceModel.Channels').[XLangMessage&lt;TSchemaBase&gt;](XLangMessage_TSchemaBase_.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>')

## XLangMessage<TSchemaBase>.XLangSchemaBaseSchemaProvider Class

Adapter class that provides [IXmlSchemaProvider](IXmlSchemaProvider.md 'Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider') support to [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived classes.

```csharp
public class XLangMessage<TSchemaBase>.XLangSchemaBaseSchemaProvider :
Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider
    where TSchemaBase : Microsoft.XLANGs.BaseTypes.SchemaBase, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage_TSchemaBase_.XLangSchemaBaseSchemaProvider.TSchemaBase'></a>

`TSchemaBase`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; XLangSchemaBaseSchemaProvider

Implements [IXmlSchemaProvider](IXmlSchemaProvider.md 'Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider')

| Explicit Interface Implementations | |
| :--- | :--- |
| [Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(XmlSchemaSet)](XLangMessage_TSchemaBase_.XLangSchemaBaseSchemaProvider.Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(XmlSchemaSet).md 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>.XLangSchemaBaseSchemaProvider.Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(System.Xml.Schema.XmlSchemaSet)') | Provides the [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') to the [schemaSet](XLangMessage_TSchemaBase_.XLangSchemaBaseSchemaProvider.Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(XmlSchemaSet).md#Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage_TSchemaBase_.XLangSchemaBaseSchemaProvider.Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>.XLangSchemaBaseSchemaProvider.Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet') and the [System.Xml.Schema.XmlSchemaType](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaType 'System.Xml.Schema.XmlSchemaType') that controls the serialization of the type. |
| [Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.Schema](XLangMessage_TSchemaBase_.XLangSchemaBaseSchemaProvider.Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.Schema.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>.XLangSchemaBaseSchemaProvider.Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.Schema') | The [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') against which to validate its XML representation. |
