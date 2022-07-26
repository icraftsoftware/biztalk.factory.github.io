#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.ContextProperties](Be.Stateless.BizTalk.ContextProperties.md 'Be.Stateless.BizTalk.ContextProperties')

## MessageContextProperty<T,TR> Class

Strong-typing wrapper for any [Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase 'Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase')-derived property.

```csharp
public class MessageContextProperty<T,TR> :
Be.Stateless.BizTalk.ContextProperties.IMessageContextProperty
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_.T'></a>

`T`

The [Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase 'Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase')-derived property to wrap.

<a name='Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_.TR'></a>

`TR`

The type of the [Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase 'Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase')-derived property.

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; MessageContextProperty<T,TR>

Implements [IMessageContextProperty](IMessageContextProperty.md 'Be.Stateless.BizTalk.ContextProperties.IMessageContextProperty')

### Remarks
To offer a truly strong-typed API over [Microsoft.BizTalk.Message.Interop.IBaseMessageContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessageContext 'Microsoft.BizTalk.Message.Interop.IBaseMessageContext') properties, this wrapper is meant to be used in
conjunction with the [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage') extension methods provided by [BaseMessage](BaseMessage.md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage').

### See Also
- [GetProperty&lt;T&gt;(this IBaseMessage, MessageContextProperty&lt;T,string&gt;)](BaseMessage.GetProperty_T_(thisIBaseMessage,MessageContextProperty_T,string_).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>)')
- [GetProperty&lt;T,TR&gt;(this IBaseMessage, MessageContextProperty&lt;T,TR&gt;)](BaseMessage.GetProperty_T,TR_(thisIBaseMessage,MessageContextProperty_T,TR_).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.GetProperty<T,TR>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>)')
- [SetProperty&lt;T&gt;(this IBaseMessage, MessageContextProperty&lt;T,string&gt;, string)](BaseMessage.SetProperty_T_(thisIBaseMessage,MessageContextProperty_T,string_,string).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>, string)')
- [SetProperty&lt;T,TV&gt;(this IBaseMessage, MessageContextProperty&lt;T,TV&gt;, TV)](BaseMessage.SetProperty_T,TV_(thisIBaseMessage,MessageContextProperty_T,TV_,TV).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.SetProperty<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>, TV)')
- [Promote&lt;T&gt;(this IBaseMessage, MessageContextProperty&lt;T,string&gt;, string)](BaseMessage.Promote_T_(thisIBaseMessage,MessageContextProperty_T,string_,string).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.Promote<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>, string)')
- [Promote&lt;T,TV&gt;(this IBaseMessage, MessageContextProperty&lt;T,TV&gt;, TV)](BaseMessage.Promote_T,TV_(thisIBaseMessage,MessageContextProperty_T,TV_,TV).md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessage.Promote<T,TV>(this Microsoft.BizTalk.Message.Interop.IBaseMessage, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>, TV)')

| Properties | |
| :--- | :--- |
| [Name](MessageContextProperty_T,TR_.Name.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.Name') | |
| [Namespace](MessageContextProperty_T,TR_.Namespace.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.Namespace') | |
| [QName](MessageContextProperty_T,TR_.QName.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.QName') | |
| [Type](MessageContextProperty_T,TR_.Type.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.Type') | |

| Operators | |
| :--- | :--- |
| [operator ==(MessageContextProperty&lt;T,TR&gt;, IConvertible)](MessageContextProperty_T,TR_.operator(MessageContextProperty_T,TR_,IConvertible).md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.op_Equality(Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, System.IConvertible)') | |
| [operator ==(MessageContextProperty&lt;T,TR&gt;, TR)](MessageContextProperty_T,TR_.operator(MessageContextProperty_T,TR_,TR).md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.op_Equality(Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, TR)') | |
| [operator &gt;(MessageContextProperty&lt;T,TR&gt;, IConvertible)](MessageContextProperty_T,TR_.operator_(MessageContextProperty_T,TR_,IConvertible).md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.op_GreaterThan(Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, System.IConvertible)') | |
| [operator &gt;(MessageContextProperty&lt;T,TR&gt;, TR)](MessageContextProperty_T,TR_.operator_(MessageContextProperty_T,TR_,TR).md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.op_GreaterThan(Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, TR)') | |
| [operator &gt;=(MessageContextProperty&lt;T,TR&gt;, IConvertible)](MessageContextProperty_T,TR_.operator_(MessageContextProperty_T,TR_,IConvertible).md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.op_GreaterThanOrEqual(Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, System.IConvertible)') | |
| [operator &gt;=(MessageContextProperty&lt;T,TR&gt;, TR)](MessageContextProperty_T,TR_.operator_(MessageContextProperty_T,TR_,TR).md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.op_GreaterThanOrEqual(Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, TR)') | |
| [operator !=(MessageContextProperty&lt;T,TR&gt;, IConvertible)](MessageContextProperty_T,TR_.operator!(MessageContextProperty_T,TR_,IConvertible).md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.op_Inequality(Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, System.IConvertible)') | |
| [operator !=(MessageContextProperty&lt;T,TR&gt;, TR)](MessageContextProperty_T,TR_.operator!(MessageContextProperty_T,TR_,TR).md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.op_Inequality(Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, TR)') | |
| [operator &lt;(MessageContextProperty&lt;T,TR&gt;, IConvertible)](MessageContextProperty_T,TR_.operator_(MessageContextProperty_T,TR_,IConvertible).md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.op_LessThan(Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, System.IConvertible)') | |
| [operator &lt;(MessageContextProperty&lt;T,TR&gt;, TR)](MessageContextProperty_T,TR_.operator_(MessageContextProperty_T,TR_,TR).md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.op_LessThan(Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, TR)') | |
| [operator &lt;=(MessageContextProperty&lt;T,TR&gt;, IConvertible)](MessageContextProperty_T,TR_.operator_(MessageContextProperty_T,TR_,IConvertible).md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.op_LessThanOrEqual(Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, System.IConvertible)') | |
| [operator &lt;=(MessageContextProperty&lt;T,TR&gt;, TR)](MessageContextProperty_T,TR_.operator_(MessageContextProperty_T,TR_,TR).md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>.op_LessThanOrEqual(Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, TR)') | |
