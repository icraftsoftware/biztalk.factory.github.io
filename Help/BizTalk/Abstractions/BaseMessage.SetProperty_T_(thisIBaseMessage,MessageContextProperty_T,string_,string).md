#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.Message.Extensions](Be.Stateless.BizTalk.Message.Extensions.md 'Be.Stateless.BizTalk.Message.Extensions').[BaseMessage](BaseMessage.md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage')

## BaseMessage.SetProperty<T>(this IBaseMessage, MessageContextProperty<T,string>, string) Method

```csharp
public static void SetProperty<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessage message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string> property, string value)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_,string).T'></a>

`T`
#### Parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_,string).message'></a>

`message` [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage')

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_,string).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[T](BaseMessage.SetProperty_T_(thisIBaseMessage,MessageContextProperty_T,string_,string).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_,string).T 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>, string).T')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_,string).value'></a>

`value` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')