#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.Message.Extensions](Be.Stateless.BizTalk.Message.Extensions.md 'Be.Stateless.BizTalk.Message.Extensions').[BaseMessage](BaseMessage.md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage')

## BaseMessage.SetProperty<T,TV>(this IBaseMessage, MessageContextProperty<T,TV>, TV) Method

```csharp
public static void SetProperty<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessage message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV> property, TV value)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new()
    where TV : struct, System.ValueType, System.ValueType;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).T'></a>

`T`

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).TV'></a>

`TV`
#### Parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).message'></a>

`message` [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage')

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[T](BaseMessage.SetProperty_T,TV_(thisIBaseMessage,MessageContextProperty_T,TV_,TV).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).T 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>, TV).T')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[TV](BaseMessage.SetProperty_T,TV_(thisIBaseMessage,MessageContextProperty_T,TV_,TV).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).TV 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>, TV).TV')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).value'></a>

`value` [TV](BaseMessage.SetProperty_T,TV_(thisIBaseMessage,MessageContextProperty_T,TV_,TV).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).TV 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>, TV).TV')