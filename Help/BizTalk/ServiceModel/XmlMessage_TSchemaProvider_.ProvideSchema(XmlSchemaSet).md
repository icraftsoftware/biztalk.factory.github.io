#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels](Be.Stateless.BizTalk.ServiceModel.Channels.md 'Be.Stateless.BizTalk.ServiceModel.Channels').[XmlMessage&lt;TSchemaProvider&gt;](XmlMessage_TSchemaProvider_.md 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>')

## XmlMessage<TSchemaProvider>.ProvideSchema(XmlSchemaSet) Method

Scaffolding method that helps a derived class to fulfill its [System.Xml.Serialization.XmlSchemaProviderAttribute](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.XmlSchemaProviderAttribute 'System.Xml.Serialization.XmlSchemaProviderAttribute')'s contract in
providing the [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema') to the [schemaSet](XmlMessage_TSchemaProvider_.ProvideSchema(XmlSchemaSet).md#Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage_TSchemaProvider_.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet 'Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage<TSchemaProvider>.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet') and the [System.Xml.Schema.XmlSchemaType](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaType 'System.Xml.Schema.XmlSchemaType') that
controls the serialization of the type.

```csharp
protected static System.Xml.Schema.XmlSchemaType ProvideSchema(System.Xml.Schema.XmlSchemaSet schemaSet);
```
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.XmlMessage_TSchemaProvider_.ProvideSchema(System.Xml.Schema.XmlSchemaSet).schemaSet'></a>

`schemaSet` [System.Xml.Schema.XmlSchemaSet](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaSet 'System.Xml.Schema.XmlSchemaSet')

The [System.Xml.Schema.XmlSchemaSet](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaSet 'System.Xml.Schema.XmlSchemaSet') that will be populated with the [System.Xml.Schema.XmlSchema](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchema 'System.Xml.Schema.XmlSchema').

#### Returns
[System.Xml.Schema.XmlSchemaType](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaType 'System.Xml.Schema.XmlSchemaType')  
The [System.Xml.Schema.XmlSchemaType](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSchemaType 'System.Xml.Schema.XmlSchemaType') that defines its data type.

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
This is a scaffolding method that is meant to be called from within the derived classes' static method identified by
the [System.Xml.Serialization.XmlSchemaProviderAttribute](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.XmlSchemaProviderAttribute 'System.Xml.Serialization.XmlSchemaProviderAttribute').