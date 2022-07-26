#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Message](Be.Stateless.BizTalk.Message.md 'Be.Stateless.BizTalk.Message').[MessageBodyFactory](MessageBodyFactory.md 'Be.Stateless.BizTalk.Message.MessageBodyFactory')

## MessageBodyFactory.Create(Type) Method

Creates a dummy instance document of a given [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived schema type [schema](MessageBodyFactory.Create(Type).md#Be.Stateless.BizTalk.Message.MessageBodyFactory.Create(System.Type).schema 'Be.Stateless.BizTalk.Message.MessageBodyFactory.Create(System.Type).schema').

```csharp
public static System.Xml.XmlDocument Create(System.Type schema);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Message.MessageBodyFactory.Create(System.Type).schema'></a>

`schema` [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')

The [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived schema type.

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
The dummy instance document as an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument').