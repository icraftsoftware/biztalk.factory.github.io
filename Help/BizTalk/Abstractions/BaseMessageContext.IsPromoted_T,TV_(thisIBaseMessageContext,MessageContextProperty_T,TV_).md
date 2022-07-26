#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.Message.Extensions](Be.Stateless.BizTalk.Message.Extensions.md 'Be.Stateless.BizTalk.Message.Extensions').[BaseMessageContext](BaseMessageContext.md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext')

## BaseMessageContext.IsPromoted<T,TV>(this IBaseMessageContext, MessageContextProperty<T,TV>) Method

```csharp
public static bool IsPromoted<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessageContext context, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV> property)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new()
    where TV : struct, System.ValueType, System.ValueType;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.IsPromoted_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_).T'></a>

`T`

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.IsPromoted_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_).TV'></a>

`TV`
#### Parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.IsPromoted_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_).context'></a>

`context` [Microsoft.BizTalk.Message.Interop.IBaseMessageContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessageContext 'Microsoft.BizTalk.Message.Interop.IBaseMessageContext')

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.IsPromoted_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[T](BaseMessageContext.IsPromoted_T,TV_(thisIBaseMessageContext,MessageContextProperty_T,TV_).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.IsPromoted_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_).T 'Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.IsPromoted<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessageContext, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>).T')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[TV](BaseMessageContext.IsPromoted_T,TV_(thisIBaseMessageContext,MessageContextProperty_T,TV_).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.IsPromoted_T,TV_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_).TV 'Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.IsPromoted<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessageContext, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>).TV')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')