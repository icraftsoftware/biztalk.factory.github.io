#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Schema](Be.Stateless.BizTalk.Xml.Schema.md 'Be.Stateless.BizTalk.Xml.Schema')

## IXmlSchemaProvider Interface

Scaffolding interface meant to help an [XmlMessage&lt;TSchemaProvider&gt;](XmlMessage_TSchemaProvider_.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>')-derived class to either get the [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') against which to validate its XML representation, or fulfill its contract with respect to the [System.Xml.Serialization.XmlSchemaProviderAttribute](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.XmlSchemaProviderAttribute 'System.Xml.Serialization.XmlSchemaProviderAttribute').

```csharp
public interface IXmlSchemaProvider
```

Derived  
&#8627; [XLangSchemaBaseSchemaProvider](XLangMessage_TSchemaBase_.XLangSchemaBaseSchemaProvider.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>.XLangSchemaBaseSchemaProvider')  
&#8627; [XmlSchemaBase](XmlSchemaBase.md 'Be.Stateless.BizTalk.Xml.Schema.XmlSchemaBase')

### Remarks
Provides the [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') to the [System.Xml.Schema.XmlSchemaSet](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaSet 'System.Xml.Schema.XmlSchemaSet') and the [System.Xml.Schema.XmlSchemaType](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaType 'System.Xml.Schema.XmlSchemaType') that controls
the serialization of the type to the .

| Properties | |
| :--- | :--- |
| [Schema](IXmlSchemaProvider.Schema.md 'Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.Schema') | The [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') against which to validate its XML representation. |

| Methods | |
| :--- | :--- |
| [ProvideSchema(XmlSchemaSet)](IXmlSchemaProvider.ProvideSchema(XmlSchemaSet).md 'Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(System.Xml.Schema.XmlSchemaSet)') | Provides the [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') to the [schemaSet](IXmlSchemaProvider.ProvideSchema(XmlSchemaSet).md#Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet 'Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet') and the [System.Xml.Schema.XmlSchemaType](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaType 'System.Xml.Schema.XmlSchemaType') that controls the serialization of the type. |
