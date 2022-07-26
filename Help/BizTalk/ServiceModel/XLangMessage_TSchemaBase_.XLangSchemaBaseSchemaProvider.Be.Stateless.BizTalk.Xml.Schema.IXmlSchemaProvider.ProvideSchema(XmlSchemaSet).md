#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels](Be.Stateless.BizTalk.ServiceModel.Channels.md 'Be.Stateless.BizTalk.ServiceModel.Channels').[XLangMessage&lt;TSchemaBase&gt;](XLangMessage_TSchemaBase_.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>').[XLangSchemaBaseSchemaProvider](XLangMessage_TSchemaBase_.XLangSchemaBaseSchemaProvider.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>.XLangSchemaBaseSchemaProvider')

## XLangMessage<TSchemaBase>.XLangSchemaBaseSchemaProvider.Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(XmlSchemaSet) Method

Provides the [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') to the [schemaSet](XLangMessage_TSchemaBase_.XLangSchemaBaseSchemaProvider.Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(XmlSchemaSet).md#Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage_TSchemaBase_.XLangSchemaBaseSchemaProvider.Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>.XLangSchemaBaseSchemaProvider.Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet') and the [System.Xml.Schema.XmlSchemaType](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaType 'System.Xml.Schema.XmlSchemaType') that
controls the serialization of the type.

```csharp
System.Xml.Schema.XmlSchemaType Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(System.Xml.Schema.XmlSchemaSet schemaSet);
```
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage_TSchemaBase_.XLangSchemaBaseSchemaProvider.Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet'></a>

`schemaSet` [System.Xml.Schema.XmlSchemaSet](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaSet 'System.Xml.Schema.XmlSchemaSet')

The [System.Xml.Schema.XmlSchemaSet](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaSet 'System.Xml.Schema.XmlSchemaSet') that will be populated with the [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema').

Implements [ProvideSchema(XmlSchemaSet)](IXmlSchemaProvider.ProvideSchema(XmlSchemaSet).md 'Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(System.Xml.Schema.XmlSchemaSet)')

### Remarks
This is a scaffolding method that is meant to be called from within the derived classes' static method identified
by the [System.Xml.Serialization.XmlSchemaProviderAttribute](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.XmlSchemaProviderAttribute 'System.Xml.Serialization.XmlSchemaProviderAttribute').