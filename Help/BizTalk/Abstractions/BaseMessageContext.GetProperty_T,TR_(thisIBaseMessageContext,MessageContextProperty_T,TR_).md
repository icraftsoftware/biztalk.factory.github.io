#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.Message.Extensions](Be.Stateless.BizTalk.Message.Extensions.md 'Be.Stateless.BizTalk.Message.Extensions').[BaseMessageContext](BaseMessageContext.md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext')

## BaseMessageContext.GetProperty<T,TR>(this IBaseMessageContext, MessageContextProperty<T,TR>) Method

```csharp
public static System.Nullable<TR> GetProperty<T,TR>(this Microsoft.BizTalk.Message.Interop.IBaseMessageContext context, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR> property)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new()
    where TR : struct, System.ValueType, System.ValueType;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.GetProperty_T,TR_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).T'></a>

`T`

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.GetProperty_T,TR_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).TR'></a>

`TR`
#### Parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.GetProperty_T,TR_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).context'></a>

`context` [Microsoft.BizTalk.Message.Interop.IBaseMessageContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessageContext 'Microsoft.BizTalk.Message.Interop.IBaseMessageContext')

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.GetProperty_T,TR_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[T](BaseMessageContext.GetProperty_T,TR_(thisIBaseMessageContext,MessageContextProperty_T,TR_).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.GetProperty_T,TR_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).T 'Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.GetProperty<T,TR>(this Microsoft.BizTalk.Message.Interop.IBaseMessageContext, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>).T')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[TR](BaseMessageContext.GetProperty_T,TR_(thisIBaseMessageContext,MessageContextProperty_T,TR_).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.GetProperty_T,TR_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).TR 'Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.GetProperty<T,TR>(this Microsoft.BizTalk.Message.Interop.IBaseMessageContext, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>).TR')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

#### Returns
[System.Nullable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Nullable-1 'System.Nullable`1')[TR](BaseMessageContext.GetProperty_T,TR_(thisIBaseMessageContext,MessageContextProperty_T,TR_).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.GetProperty_T,TR_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).TR 'Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.GetProperty<T,TR>(this Microsoft.BizTalk.Message.Interop.IBaseMessageContext, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>).TR')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Nullable-1 'System.Nullable`1')