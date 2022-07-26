#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels](Be.Stateless.BizTalk.ServiceModel.Channels.md 'Be.Stateless.BizTalk.ServiceModel.Channels')

## XmlMessage Class

Represents an [System.Xml.Serialization.IXmlSerializable](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.IXmlSerializable 'System.Xml.Serialization.IXmlSerializable') unit of communication between endpoints in a distributed environment.

```csharp
public class XmlMessage :
System.Xml.Serialization.IXmlSerializable
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; XmlMessage

Derived  
&#8627; [EmptyXmlMessage](EmptyXmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.EmptyXmlMessage')  
&#8627; [XmlMessage&lt;TSchemaProvider&gt;](XmlMessage_TSchemaProvider_.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>')

Implements [System.Xml.Serialization.IXmlSerializable](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.IXmlSerializable 'System.Xml.Serialization.IXmlSerializable')

| Properties | |
| :--- | :--- |
| [Action](XmlMessage.Action.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage.Action') | Gets a description of how the message should be processed. |
| [RawXmlBody](XmlMessage.RawXmlBody.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage.RawXmlBody') | |
| [Version](XmlMessage.Version.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage.Version') | Gets the SOAP version of the message. |

| Methods | |
| :--- | :--- |
| [GetReaderAtContent()](XmlMessage.GetReaderAtContent().md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage.GetReaderAtContent()') | Gets the [System.Xml.XmlReader](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlReader 'System.Xml.XmlReader') that accesses the body of this message. |
| [GetSchema()](XmlMessage.GetSchema().md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage.GetSchema()') | This method is reserved and should not be used. When implementing the [System.Xml.Serialization.IXmlSerializable](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.IXmlSerializable 'System.Xml.Serialization.IXmlSerializable') interface, you should return `null` from this method, and instead, if specifying a custom schema is required, apply the [System.Xml.Serialization.XmlSchemaProviderAttribute](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.XmlSchemaProviderAttribute 'System.Xml.Serialization.XmlSchemaProviderAttribute') to the class. |
| [ReadXml(XmlReader)](XmlMessage.ReadXml(XmlReader).md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage.ReadXml(System.Xml.XmlReader)') | Generates an object from its XML representation. |
| [WriteXml(XmlWriter)](XmlMessage.WriteXml(XmlWriter).md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage.WriteXml(System.Xml.XmlWriter)') | Converts an object into its XML representation. |
