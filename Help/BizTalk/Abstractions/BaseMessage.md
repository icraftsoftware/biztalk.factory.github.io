#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.Message.Extensions](Be.Stateless.BizTalk.Message.Extensions.md 'Be.Stateless.BizTalk.Message.Extensions')

## BaseMessage Class

Various [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage') extension methods that allow for shorter and <b>type-safe</b> statements.

```csharp
public static class BaseMessage
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; BaseMessage

### Remarks

Noticeably, offers <b>type-safe</b> and easier to use [Microsoft.BizTalk.Message.Interop.IBaseMessageContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessageContext 'Microsoft.BizTalk.Message.Interop.IBaseMessageContext') property getters,
setters, and promoters.

| Methods | |
| :--- | :--- |
| [DeleteProperty&lt;T,TR&gt;(this IBaseMessage, MessageContextProperty&lt;T,TR&gt;)](BaseMessage.DeleteProperty_T,TR_(thisIBaseMessage,MessageContextProperty_T,TR_).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.DeleteProperty<T,TR>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>)') | |
| [DeleteProperty&lt;T&gt;(this IBaseMessage, MessageContextProperty&lt;T,string&gt;)](BaseMessage.DeleteProperty_T_(thisIBaseMessage,MessageContextProperty_T,string_).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.DeleteProperty<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>)') | |
| [DeleteProperty&lt;T&gt;(this XLANGMessage, MessageContextProperty&lt;T,object&gt;)](BaseMessage.DeleteProperty_T_(thisXLANGMessage,MessageContextProperty_T,object_).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.DeleteProperty<T>(this Microsoft.XLANGs.BaseTypes.XLANGMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,object>)') | |
| [GetProperty&lt;T,TR&gt;(this IBaseMessage, MessageContextProperty&lt;T,TR&gt;)](BaseMessage.GetProperty_T,TR_(thisIBaseMessage,MessageContextProperty_T,TR_).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty<T,TR>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>)') | |
| [GetProperty&lt;T,TR&gt;(this XLANGMessage, MessageContextProperty&lt;T,TR&gt;)](BaseMessage.GetProperty_T,TR_(thisXLANGMessage,MessageContextProperty_T,TR_).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty<T,TR>(this Microsoft.XLANGs.BaseTypes.XLANGMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>)') | |
| [GetProperty&lt;T&gt;(this IBaseMessage, MessageContextProperty&lt;T,string&gt;)](BaseMessage.GetProperty_T_(thisIBaseMessage,MessageContextProperty_T,string_).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>)') | |
| [GetProperty&lt;T&gt;(this XLANGMessage, MessageContextProperty&lt;T,string&gt;)](BaseMessage.GetProperty_T_(thisXLANGMessage,MessageContextProperty_T,string_).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty<T>(this Microsoft.XLANGs.BaseTypes.XLANGMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>)') | |
| [IsPromoted&lt;T,TV&gt;(this IBaseMessage, MessageContextProperty&lt;T,TV&gt;)](BaseMessage.IsPromoted_T,TV_(thisIBaseMessage,MessageContextProperty_T,TV_).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.IsPromoted<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>)') | |
| [IsPromoted&lt;T&gt;(this IBaseMessage, MessageContextProperty&lt;T,string&gt;)](BaseMessage.IsPromoted_T_(thisIBaseMessage,MessageContextProperty_T,string_).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.IsPromoted<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>)') | |
| [Promote&lt;T,TV&gt;(this IBaseMessage, MessageContextProperty&lt;T,TV&gt;, TV)](BaseMessage.Promote_T,TV_(thisIBaseMessage,MessageContextProperty_T,TV_,TV).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.Promote<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>, TV)') | |
| [Promote&lt;T&gt;(this IBaseMessage, MessageContextProperty&lt;T,string&gt;, string)](BaseMessage.Promote_T_(thisIBaseMessage,MessageContextProperty_T,string_,string).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.Promote<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>, string)') | |
| [SetProperty&lt;T,TV&gt;(this IBaseMessage, MessageContextProperty&lt;T,TV&gt;, TV)](BaseMessage.SetProperty_T,TV_(thisIBaseMessage,MessageContextProperty_T,TV_,TV).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>, TV)') | |
| [SetProperty&lt;T,TV&gt;(this XLANGMessage, MessageContextProperty&lt;T,TV&gt;, TV)](BaseMessage.SetProperty_T,TV_(thisXLANGMessage,MessageContextProperty_T,TV_,TV).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty<T,TV>(this Microsoft.XLANGs.BaseTypes.XLANGMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>, TV)') | |
| [SetProperty&lt;T&gt;(this IBaseMessage, MessageContextProperty&lt;T,string&gt;, string)](BaseMessage.SetProperty_T_(thisIBaseMessage,MessageContextProperty_T,string_,string).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>, string)') | |
| [SetProperty&lt;T&gt;(this XLANGMessage, MessageContextProperty&lt;T,string&gt;, string)](BaseMessage.SetProperty_T_(thisXLANGMessage,MessageContextProperty_T,string_,string).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty<T>(this Microsoft.XLANGs.BaseTypes.XLANGMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>, string)') | |
