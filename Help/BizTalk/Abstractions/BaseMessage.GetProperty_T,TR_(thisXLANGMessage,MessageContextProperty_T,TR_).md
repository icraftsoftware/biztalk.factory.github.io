#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.Message.Extensions](Be.Stateless.BizTalk.Message.Extensions.md 'Be.Stateless.BizTalk.Message.Extensions').[BaseMessage](BaseMessage.md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage')

## BaseMessage.GetProperty<T,TR>(this XLANGMessage, MessageContextProperty<T,TR>) Method

```csharp
public static System.Nullable<TR> GetProperty<T,TR>(this Microsoft.XLANGs.BaseTypes.XLANGMessage message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR> property)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new()
    where TR : struct, System.ValueType, System.ValueType;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty_T,TR_(thisMicrosoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).T'></a>

`T`

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty_T,TR_(thisMicrosoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).TR'></a>

`TR`
#### Parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty_T,TR_(thisMicrosoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).message'></a>

`message` [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty_T,TR_(thisMicrosoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[T](BaseMessage.GetProperty_T,TR_(thisXLANGMessage,MessageContextProperty_T,TR_).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty_T,TR_(thisMicrosoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).T 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty<T,TR>(this Microsoft.XLANGs.BaseTypes.XLANGMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>).T')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[TR](BaseMessage.GetProperty_T,TR_(thisXLANGMessage,MessageContextProperty_T,TR_).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty_T,TR_(thisMicrosoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).TR 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty<T,TR>(this Microsoft.XLANGs.BaseTypes.XLANGMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>).TR')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

#### Returns
[System.Nullable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Nullable-1 'System.Nullable`1')[TR](BaseMessage.GetProperty_T,TR_(thisXLANGMessage,MessageContextProperty_T,TR_).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty_T,TR_(thisMicrosoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).TR 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty<T,TR>(this Microsoft.XLANGs.BaseTypes.XLANGMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>).TR')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Nullable-1 'System.Nullable`1')