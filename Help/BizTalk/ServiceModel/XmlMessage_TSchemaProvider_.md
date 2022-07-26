#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels](Be.Stateless.BizTalk.ServiceModel.Channels.md 'Be.Stateless.BizTalk.ServiceModel.Channels')

## XmlMessage<TSchemaProvider> Class

Represents an [System.Xml.Serialization.IXmlSerializable](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.IXmlSerializable 'System.Xml.Serialization.IXmlSerializable') unit of communication between endpoints in a distributed environment whose
content is defined by an [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') that a [TSchemaProvider](XmlMessage_TSchemaProvider_.md#Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage_TSchemaProvider_.TSchemaProvider 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>.TSchemaProvider') can provide.

```csharp
public abstract class XmlMessage<TSchemaProvider> : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage
    where TSchemaProvider : Be.Stateless.BizTalk.Xml.Schema.IXmlSchemaProvider, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage_TSchemaProvider_.TSchemaProvider'></a>

`TSchemaProvider`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') &#129106; XmlMessage<TSchemaProvider>

Derived  
&#8627; [XLangMessage&lt;TSchemaBase&gt;](XLangMessage_TSchemaBase_.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>')

### Example

```csharp
[XmlSchemaProvider("GetSchema")]
public class CalculatorArguments : XmlMessage<CalculatorMessageSchema.Arguments> {
   public new static XmlSchemaType GetSchema(XmlSchemaSet schemaSet) {
      return ProvideSchema(schemaSet);
   }

   ...

}
```

### Remarks
This class helps its derived classes to fulfill the [System.Xml.Serialization.XmlSchemaProviderAttribute](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.XmlSchemaProviderAttribute 'System.Xml.Serialization.XmlSchemaProviderAttribute')'s contract, see [ProvideSchema(XmlSchemaSet)](XmlMessage_TSchemaProvider_.ProvideSchema(XmlSchemaSet).md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>.ProvideSchema(System.Xml.Schema.XmlSchemaSet)').

| Constructors | |
| :--- | :--- |
| [XmlMessage()](XmlMessage_TSchemaProvider_.XmlMessage().md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>.XmlMessage()') | Initializes a new instance of the [XmlMessage&lt;TSchemaProvider&gt;](XmlMessage_TSchemaProvider_.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>') class that will skip XML validation. |
| [XmlMessage(XmlSchemaContentProcessing)](XmlMessage_TSchemaProvider_.XmlMessage(XmlSchemaContentProcessing).md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>.XmlMessage(System.Xml.Schema.XmlSchemaContentProcessing)') | Initializes a new instance of the [XmlMessage&lt;TSchemaProvider&gt;](XmlMessage_TSchemaProvider_.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>') class that will validate its XML representation. |

| Methods | |
| :--- | :--- |
| [ProvideSchema(XmlSchemaSet)](XmlMessage_TSchemaProvider_.ProvideSchema(XmlSchemaSet).md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>.ProvideSchema(System.Xml.Schema.XmlSchemaSet)') | Scaffolding method that helps a derived class to fulfill its [System.Xml.Serialization.XmlSchemaProviderAttribute](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.XmlSchemaProviderAttribute 'System.Xml.Serialization.XmlSchemaProviderAttribute')'s contract in providing the [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') to the [schemaSet](XmlMessage_TSchemaProvider_.ProvideSchema(XmlSchemaSet).md#Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage_TSchemaProvider_.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet') and the [System.Xml.Schema.XmlSchemaType](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaType 'System.Xml.Schema.XmlSchemaType') that controls the serialization of the type. |
| [ReadXml(XmlReader)](XmlMessage_TSchemaProvider_.ReadXml(XmlReader).md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>.ReadXml(System.Xml.XmlReader)') | Generates an object from its XML representation that will be validated while being read if validation has been enforced at construction time. |
