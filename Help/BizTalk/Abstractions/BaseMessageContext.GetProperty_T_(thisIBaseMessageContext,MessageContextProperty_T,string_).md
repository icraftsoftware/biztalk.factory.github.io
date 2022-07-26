#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.Message.Extensions](Be.Stateless.BizTalk.Message.Extensions.md 'Be.Stateless.BizTalk.Message.Extensions').[BaseMessageContext](BaseMessageContext.md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext')

## BaseMessageContext.GetProperty<T>(this IBaseMessageContext, MessageContextProperty<T,string>) Method

```csharp
public static string GetProperty<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessageContext context, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string> property)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.GetProperty_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_).T'></a>

`T`
#### Parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.GetProperty_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_).context'></a>

`context` [Microsoft.BizTalk.Message.Interop.IBaseMessageContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessageContext 'Microsoft.BizTalk.Message.Interop.IBaseMessageContext')

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.GetProperty_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[T](BaseMessageContext.GetProperty_T_(thisIBaseMessageContext,MessageContextProperty_T,string_).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.GetProperty_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessageContext,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_).T 'Be.Stateless.BizTalk.Message.Extensions.BaseMessageContext.GetProperty<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessageContext, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>).T')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')