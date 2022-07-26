#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Schema](Be.Stateless.BizTalk.Xml.Schema.md 'Be.Stateless.BizTalk.Xml.Schema').[XmlSchemaBase](XmlSchemaBase.md 'Be.Stateless.BizTalk.Xml.Schema.XmlSchemaBase')

## XmlSchemaBase.ProvideSchema(XmlSchemaSet) Method

Provides the [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') to the [schemaSet](XmlSchemaBase.ProvideSchema(XmlSchemaSet).md#Be.Stateless.BizTalk.Xml.Schema.XmlSchemaBase.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet 'Be.Stateless.BizTalk.Xml.Schema.XmlSchemaBase.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet') and the [System.Xml.Schema.XmlSchemaType](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaType 'System.Xml.Schema.XmlSchemaType') that
controls the serialization of the type.

```csharp
public System.Xml.Schema.XmlSchemaType ProvideSchema(System.Xml.Schema.XmlSchemaSet schemaSet);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Xml.Schema.XmlSchemaBase.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet'></a>

`schemaSet` [System.Xml.Schema.XmlSchemaSet](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaSet 'System.Xml.Schema.XmlSchemaSet')

The [System.Xml.Schema.XmlSchemaSet](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaSet 'System.Xml.Schema.XmlSchemaSet') that will be populated with the [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema').

Implements [ProvideSchema(XmlSchemaSet)](IXmlSchemaProvider.ProvideSchema(XmlSchemaSet).md 'Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider.ProvideSchema(System.Xml.Schema.XmlSchemaSet)')

#### Returns
[System.Xml.Schema.XmlSchemaType](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaType 'System.Xml.Schema.XmlSchemaType')  
The [System.Xml.Schema.XmlSchemaType](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaType 'System.Xml.Schema.XmlSchemaType') that defines its data type.

### Remarks
This is a scaffolding method that is meant to be called from within the derived classes' static method identified by
the [System.Xml.Serialization.XmlSchemaProviderAttribute](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.XmlSchemaProviderAttribute 'System.Xml.Serialization.XmlSchemaProviderAttribute').