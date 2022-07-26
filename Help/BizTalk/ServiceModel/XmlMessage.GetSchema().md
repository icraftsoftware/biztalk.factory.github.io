#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels](Be.Stateless.BizTalk.ServiceModel.Channels.md 'Be.Stateless.BizTalk.ServiceModel.Channels').[XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage')

## XmlMessage.GetSchema() Method

This method is reserved and should not be used. When implementing the [System.Xml.Serialization.IXmlSerializable](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.IXmlSerializable 'System.Xml.Serialization.IXmlSerializable') interface, you
should return `null` from this method, and instead, if specifying a custom schema is required, apply the [System.Xml.Serialization.XmlSchemaProviderAttribute](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.XmlSchemaProviderAttribute 'System.Xml.Serialization.XmlSchemaProviderAttribute') to the class.

```csharp
public virtual System.Xml.Schema.XmlSchema GetSchema();
```

Implements [GetSchema()](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.IXmlSerializable.GetSchema 'System.Xml.Serialization.IXmlSerializable.GetSchema')

#### Returns
[System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema')  
An [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') that describes the XML representation of the object that is produced by the [System.Xml.Serialization.IXmlSerializable.WriteXml(System.Xml.XmlWriter)](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.IXmlSerializable.WriteXml#System_Xml_Serialization_IXmlSerializable_WriteXml_System_Xml_XmlWriter_ 'System.Xml.Serialization.IXmlSerializable.WriteXml(System.Xml.XmlWriter)') method and consumed by the [System.Xml.Serialization.IXmlSerializable.ReadXml(System.Xml.XmlReader)](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.IXmlSerializable.ReadXml#System_Xml_Serialization_IXmlSerializable_ReadXml_System_Xml_XmlReader_ 'System.Xml.Serialization.IXmlSerializable.ReadXml(System.Xml.XmlReader)') method.