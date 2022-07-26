#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Message](Be.Stateless.BizTalk.Message.md 'Be.Stateless.BizTalk.Message')

## MessageBodyFactory Class

```csharp
public static class MessageBodyFactory
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; MessageBodyFactory

| Methods | |
| :--- | :--- |
| [Create(Type)](MessageBodyFactory.Create(Type).md 'Be.Stateless.BizTalk.Message.MessageBodyFactory.Create(System.Type)') | Creates a dummy instance document of a given [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived schema type [schema](MessageBodyFactory.Create(Type).md#Be.Stateless.BizTalk.Message.MessageBodyFactory.Create(System.Type).schema 'Be.Stateless.BizTalk.Message.MessageBodyFactory.Create(System.Type).schema'). |
| [Create&lt;T&gt;()](MessageBodyFactory.Create_T_().md 'Be.Stateless.BizTalk.Message.MessageBodyFactory.Create<T>()') | Creates a dummy instance document of a given [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived schema type [T](MessageBodyFactory.Create_T_().md#Be.Stateless.BizTalk.Message.MessageBodyFactory.Create_T_().T 'Be.Stateless.BizTalk.Message.MessageBodyFactory.Create<T>().T'). |
| [Create&lt;T&gt;(string)](MessageBodyFactory.Create_T_(string).md 'Be.Stateless.BizTalk.Message.MessageBodyFactory.Create<T>(string)') | Creates an [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') from a given [content](MessageBodyFactory.Create_T_(string).md#Be.Stateless.BizTalk.Message.MessageBodyFactory.Create_T_(string).content 'Be.Stateless.BizTalk.Message.MessageBodyFactory.Create<T>(string).content') and ensures its validity against a given [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived schema type [T](MessageBodyFactory.Create_T_(string).md#Be.Stateless.BizTalk.Message.MessageBodyFactory.Create_T_(string).T 'Be.Stateless.BizTalk.Message.MessageBodyFactory.Create<T>(string).T'). |
| [CreateEnvelope&lt;TE,TC&gt;(string)](MessageBodyFactory.CreateEnvelope_TE,TC_(string).md 'Be.Stateless.BizTalk.Message.MessageBodyFactory.CreateEnvelope<TE,TC>(string)') | Creates a envelope document with content for a given [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived envelope schema type [TE](MessageBodyFactory.CreateEnvelope_TE,TC_(string).md#Be.Stateless.BizTalk.Message.MessageBodyFactory.CreateEnvelope_TE,TC_(string).TE 'Be.Stateless.BizTalk.Message.MessageBodyFactory.CreateEnvelope<TE,TC>(string).TE') and [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived content schema type [TC](MessageBodyFactory.CreateEnvelope_TE,TC_(string).md#Be.Stateless.BizTalk.Message.MessageBodyFactory.CreateEnvelope_TE,TC_(string).TC 'Be.Stateless.BizTalk.Message.MessageBodyFactory.CreateEnvelope<TE,TC>(string).TC') . |