#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.Message.Extensions](Be.Stateless.BizTalk.Message.Extensions.md 'Be.Stateless.BizTalk.Message.Extensions').[BaseMessageContext](BaseMessageContext.md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext')

## BaseMessageContext.Promote<T,TV>(this IBaseMessageContext, MessageContextProperty<T,TV>, TV) Method

```csharp
public static void Promote<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessageContext context, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV> property, TV value)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new()
    where TV : struct, System.ValueType, System.ValueType;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).T'></a>

`T`

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).TV'></a>

`TV`
#### Parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).context'></a>

`context` [Microsoft.BizTalk.Message.Interop.IBaseMessageContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessageContext 'Microsoft.BizTalk.Message.Interop.IBaseMessageContext')

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[T](BaseMessageContext.Promote_T,TV_(thisIBaseMessageContext,MessageContextProperty_T,TV_,TV).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).T 'Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessageContext, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>, TV).T')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[TV](BaseMessageContext.Promote_T,TV_(thisIBaseMessageContext,MessageContextProperty_T,TV_,TV).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).TV 'Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessageContext, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>, TV).TV')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).value'></a>

`value` [TV](BaseMessageContext.Promote_T,TV_(thisIBaseMessageContext,MessageContextProperty_T,TV_,TV).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).TV 'Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessageContext, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>, TV).TV')