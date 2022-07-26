#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels](Be.Stateless.BizTalk.ServiceModel.Channels.md 'Be.Stateless.BizTalk.ServiceModel.Channels').[EmptyXmlMessage](EmptyXmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.EmptyXmlMessage')

## EmptyXmlMessage.WriteXml(XmlWriter) Method

Converts an object into its XML representation.

```csharp
public override void WriteXml(System.Xml.XmlWriter writer);
```
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.EmptyXmlMessage.WriteXml(System.Xml.XmlWriter).writer'></a>

`writer` [System.Xml.XmlWriter](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlWriter 'System.Xml.XmlWriter')

The [System.Xml.XmlWriter](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlWriter 'System.Xml.XmlWriter') stream to which the object is serialized.

Implements [WriteXml(XmlWriter)](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.IXmlSerializable.WriteXml#System_Xml_Serialization_IXmlSerializable_WriteXml_System_Xml_XmlWriter_ 'System.Xml.Serialization.IXmlSerializable.WriteXml(System.Xml.XmlWriter)')

### Remarks
Because the intent is to work at the XML level of messages complying to a message contract (by opposition to a
DataContract), where we want to keep control on the whole XML, this method skips the root XML element as the actual
root element surrounding the response [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') will be provided by WCF.