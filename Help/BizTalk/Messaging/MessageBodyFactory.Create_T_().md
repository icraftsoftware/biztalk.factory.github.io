#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Message](Be.Stateless.BizTalk.Message.md 'Be.Stateless.BizTalk.Message').[MessageBodyFactory](MessageBodyFactory.md 'Be.Stateless.BizTalk.Message.MessageBodyFactory')

## MessageBodyFactory.Create<T>() Method

Creates a dummy instance document of a given [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived schema type [T](MessageBodyFactory.Create_T_().md#Be.Stateless.BizTalk.Message.MessageBodyFactory.Create_T_().T 'Be.Stateless.BizTalk.Message.MessageBodyFactory.Create<T>().T').

```csharp
public static System.Xml.XmlDocument Create<T>()
    where T : Microsoft.XLANGs.BaseTypes.SchemaBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Message.MessageBodyFactory.Create_T_().T'></a>

`T`

The [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived schema type.

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
The dummy instance document as an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument').