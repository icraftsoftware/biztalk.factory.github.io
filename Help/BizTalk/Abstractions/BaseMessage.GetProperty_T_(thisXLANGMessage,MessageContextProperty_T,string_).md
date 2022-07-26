#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.Message.Extensions](Be.Stateless.BizTalk.Message.Extensions.md 'Be.Stateless.BizTalk.Message.Extensions').[BaseMessage](BaseMessage.md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage')

## BaseMessage.GetProperty<T>(this XLANGMessage, MessageContextProperty<T,string>) Method

```csharp
public static string GetProperty<T>(this Microsoft.XLANGs.BaseTypes.XLANGMessage message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string> property)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty_T_(thisMicrosoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_).T'></a>

`T`
#### Parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty_T_(thisMicrosoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_).message'></a>

`message` [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty_T_(thisMicrosoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[T](BaseMessage.GetProperty_T_(thisXLANGMessage,MessageContextProperty_T,string_).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty_T_(thisMicrosoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_).T 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty<T>(this Microsoft.XLANGs.BaseTypes.XLANGMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>).T')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')