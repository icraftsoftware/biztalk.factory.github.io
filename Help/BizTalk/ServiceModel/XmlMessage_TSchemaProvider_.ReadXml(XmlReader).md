#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels](Be.Stateless.BizTalk.ServiceModel.Channels.md 'Be.Stateless.BizTalk.ServiceModel.Channels').[XmlMessage&lt;TSchemaProvider&gt;](XmlMessage_TSchemaProvider_.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>')

## XmlMessage<TSchemaProvider>.ReadXml(XmlReader) Method

Generates an object from its XML representation that will be validated while being read if validation has been
enforced at construction time.

```csharp
public override void ReadXml(System.Xml.XmlReader reader);
```
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage_TSchemaProvider_.ReadXml(System.Xml.XmlReader).reader'></a>

`reader` [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader')

The [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') stream from which the object is deserialized.

Implements [ReadXml(XmlReader)](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.IXmlSerializable.ReadXml#System_Xml_Serialization_IXmlSerializable_ReadXml_System_Xml_XmlReader_ 'System.Xml.Serialization.IXmlSerializable.ReadXml(System.Xml.XmlReader)')