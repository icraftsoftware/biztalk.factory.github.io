#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.Message.Extensions](Be.Stateless.BizTalk.Message.Extensions.md 'Be.Stateless.BizTalk.Message.Extensions').[BaseMessageContext](BaseMessageContext.md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext')

## BaseMessageContext.Promote<T>(this IBaseMessageContext, MessageContextProperty<T,string>, string) Method

```csharp
public static void Promote<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessageContext context, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string> property, string value)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_,string).T'></a>

`T`
#### Parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_,string).context'></a>

`context` [Microsoft.BizTalk.Message.Interop.IBaseMessageContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessageContext 'Microsoft.BizTalk.Message.Interop.IBaseMessageContext')

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_,string).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[T](BaseMessageContext.Promote_T_(thisIBaseMessageContext,MessageContextProperty_T,string_,string).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_,string).T 'Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessageContext, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>, string).T')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.Promote_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_,string).value'></a>

`value` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')