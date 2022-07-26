#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Message](Be.Stateless.BizTalk.Message.md 'Be.Stateless.BizTalk.Message').[MessageBodyFactory](MessageBodyFactory.md 'Be.Stateless.BizTalk.Message.MessageBodyFactory')

## MessageBodyFactory.Create<T>(string) Method

Creates an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') from a given [content](MessageBodyFactory.Create_T_(string).md#Be.Stateless.BizTalk.Message.MessageBodyFactory.Create_T_(string).content 'Be.Stateless.BizTalk.Message.MessageBodyFactory.Create<T>(string).content') and ensures its validity against a given
[Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived schema type [T](MessageBodyFactory.Create_T_(string).md#Be.Stateless.BizTalk.Message.MessageBodyFactory.Create_T_(string).T 'Be.Stateless.BizTalk.Message.MessageBodyFactory.Create<T>(string).T').

```csharp
public static System.Xml.XmlDocument Create<T>(string content)
    where T : Microsoft.XLANGs.BaseTypes.SchemaBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Message.MessageBodyFactory.Create_T_(string).T'></a>

`T`

The [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived schema type.
#### Parameters

<a name='Be.Stateless.BizTalk.Message.MessageBodyFactory.Create_T_(string).content'></a>

`content` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The instance document content.

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
The valid instance document as an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument').