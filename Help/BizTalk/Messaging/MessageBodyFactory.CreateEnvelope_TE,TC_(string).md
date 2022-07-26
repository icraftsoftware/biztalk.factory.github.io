#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Message](Be.Stateless.BizTalk.Message.md 'Be.Stateless.BizTalk.Message').[MessageBodyFactory](MessageBodyFactory.md 'Be.Stateless.BizTalk.Message.MessageBodyFactory')

## MessageBodyFactory.CreateEnvelope<TE,TC>(string) Method

Creates a envelope document with content for a given [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived envelope schema type
[TE](MessageBodyFactory.CreateEnvelope_TE,TC_(string).md#Be.Stateless.BizTalk.Message.MessageBodyFactory.CreateEnvelope_TE,TC_(string).TE 'Be.Stateless.BizTalk.Message.MessageBodyFactory.CreateEnvelope<TE,TC>(string).TE') and [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived content schema type [TC](MessageBodyFactory.CreateEnvelope_TE,TC_(string).md#Be.Stateless.BizTalk.Message.MessageBodyFactory.CreateEnvelope_TE,TC_(string).TC 'Be.Stateless.BizTalk.Message.MessageBodyFactory.CreateEnvelope<TE,TC>(string).TC') .

```csharp
public static System.Xml.XmlDocument CreateEnvelope<TE,TC>(string content)
    where TE : Microsoft.XLANGs.BaseTypes.SchemaBase, new()
    where TC : Microsoft.XLANGs.BaseTypes.SchemaBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Message.MessageBodyFactory.CreateEnvelope_TE,TC_(string).TE'></a>

`TE`

The [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived envelope schema type.

<a name='Be.Stateless.BizTalk.Message.MessageBodyFactory.CreateEnvelope_TE,TC_(string).TC'></a>

`TC`

The [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived content schema type.
#### Parameters

<a name='Be.Stateless.BizTalk.Message.MessageBodyFactory.CreateEnvelope_TE,TC_(string).content'></a>

`content` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

#### Returns
[System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')  
The envelope document with its content as an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument').