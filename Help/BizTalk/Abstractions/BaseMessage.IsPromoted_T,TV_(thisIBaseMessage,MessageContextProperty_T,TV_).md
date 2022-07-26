#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.Message.Extensions](Be.Stateless.BizTalk.Message.Extensions.md 'Be.Stateless.BizTalk.Message.Extensions').[BaseMessage](BaseMessage.md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage')

## BaseMessage.IsPromoted<T,TV>(this IBaseMessage, MessageContextProperty<T,TV>) Method

```csharp
public static bool IsPromoted<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessage message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV> property)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new()
    where TV : struct, System.ValueType, System.ValueType;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.IsPromoted_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_).T'></a>

`T`

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.IsPromoted_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_).TV'></a>

`TV`
#### Parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.IsPromoted_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_).message'></a>

`message` [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage')

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.IsPromoted_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[T](BaseMessage.IsPromoted_T,TV_(thisIBaseMessage,MessageContextProperty_T,TV_).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessage.IsPromoted_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_).T 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.IsPromoted<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>).T')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[TV](BaseMessage.IsPromoted_T,TV_(thisIBaseMessage,MessageContextProperty_T,TV_).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessage.IsPromoted_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_).TV 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.IsPromoted<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>).TV')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')