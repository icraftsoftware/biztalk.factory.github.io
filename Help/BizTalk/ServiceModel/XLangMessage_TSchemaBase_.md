#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels](Be.Stateless.BizTalk.ServiceModel.Channels.md 'Be.Stateless.BizTalk.ServiceModel.Channels')

## XLangMessage<TSchemaBase> Class

Represents an [System.Xml.Serialization.IXmlSerializable](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.IXmlSerializable 'System.Xml.Serialization.IXmlSerializable') unit of communication between endpoints in a distributed environment whose
content is defined by an [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived XML schema.

```csharp
public class XLangMessage<TSchemaBase> : Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>.XLangSchemaBaseSchemaProvider>
    where TSchemaBase : Microsoft.XLANGs.BaseTypes.SchemaBase, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage_TSchemaBase_.TSchemaBase'></a>

`TSchemaBase`

The [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived XML schema.

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [XmlMessage](XmlMessage.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage') &#129106; [Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage&lt;](XmlMessage_TSchemaProvider_.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>')[Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage.XLangSchemaBaseSchemaProvider&lt;](XLangMessage_TSchemaBase_.XLangSchemaBaseSchemaProvider.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>.XLangSchemaBaseSchemaProvider')[TSchemaBase](XLangMessage_TSchemaBase_.md#Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage_TSchemaBase_.TSchemaBase 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>.TSchemaBase')[&gt;](XLangMessage_TSchemaBase_.XLangSchemaBaseSchemaProvider.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>.XLangSchemaBaseSchemaProvider')[&gt;](XmlMessage_TSchemaProvider_.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>') &#129106; XLangMessage<TSchemaBase>

### Example

```csharp
[XmlSchemaProvider("GetSchema")]
public class CalculatorArguments : XLangMessage<CalculatorMessageSchema.Arguments> {
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
| [XLangMessage()](XLangMessage_TSchemaBase_.XLangMessage().md 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>.XLangMessage()') | Initializes a new instance of the [XLangMessage&lt;TSchemaBase&gt;](XLangMessage_TSchemaBase_.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>') class that will skip XML validation. |
| [XLangMessage(XmlSchemaContentProcessing)](XLangMessage_TSchemaBase_.XLangMessage(XmlSchemaContentProcessing).md 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>.XLangMessage(System.Xml.Schema.XmlSchemaContentProcessing)') | Initializes a new instance of the [XLangMessage&lt;TSchemaBase&gt;](XLangMessage_TSchemaBase_.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>') class that will validate its XML representation. |

| Methods | |
| :--- | :--- |
| [GetXmlSchemaForXLangMessage(XmlSchemaSet)](XLangMessage_TSchemaBase_.GetXmlSchemaForXLangMessage(XmlSchemaSet).md 'Be.Stateless.BizTalk.ServiceModel.Channels.XLangMessage<TSchemaBase>.GetXmlSchemaForXLangMessage(System.Xml.Schema.XmlSchemaSet)') | |
