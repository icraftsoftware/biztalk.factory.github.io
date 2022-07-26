#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Message.Extensions](Be.Stateless.BizTalk.Message.Extensions.md 'Be.Stateless.BizTalk.Message.Extensions').[BaseMessagePartExtensions](BaseMessagePartExtensions.md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions')

## BaseMessagePartExtensions.WrapOriginalDataStream<T>(this IBaseMessagePart, Func<Stream,T>, IResourceTracker) Method

Wraps this message part's original data stream in another stream returned by the [wrapper](BaseMessagePartExtensions.WrapOriginalDataStream_T_(thisIBaseMessagePart,Func_Stream,T_,IResourceTracker).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.WrapOriginalDataStream_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessagePart,System.Func_System.IO.Stream,T_,Microsoft.BizTalk.Component.Interop.IResourceTracker).wrapper 'Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.WrapOriginalDataStream<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessagePart, System.Func<System.IO.Stream,T>, Microsoft.BizTalk.Component.Interop.IResourceTracker).wrapper') delegate.

```csharp
public static T WrapOriginalDataStream<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessagePart messagePart, System.Func<System.IO.Stream,T> wrapper, Microsoft.BizTalk.Component.Interop.IResourceTracker tracker)
    where T : System.IO.Stream;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.WrapOriginalDataStream_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessagePart,System.Func_System.IO.Stream,T_,Microsoft.BizTalk.Component.Interop.IResourceTracker).T'></a>

`T`
#### Parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.WrapOriginalDataStream_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessagePart,System.Func_System.IO.Stream,T_,Microsoft.BizTalk.Component.Interop.IResourceTracker).messagePart'></a>

`messagePart` [Microsoft.BizTalk.Message.Interop.IBaseMessagePart](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessagePart 'Microsoft.BizTalk.Message.Interop.IBaseMessagePart')

The part whose original data stream is wrapped.

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.WrapOriginalDataStream_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessagePart,System.Func_System.IO.Stream,T_,Microsoft.BizTalk.Component.Interop.IResourceTracker).wrapper'></a>

`wrapper` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')[T](BaseMessagePartExtensions.WrapOriginalDataStream_T_(thisIBaseMessagePart,Func_Stream,T_,IResourceTracker).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.WrapOriginalDataStream_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessagePart,System.Func_System.IO.Stream,T_,Microsoft.BizTalk.Component.Interop.IResourceTracker).T 'Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.WrapOriginalDataStream<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessagePart, System.Func<System.IO.Stream,T>, Microsoft.BizTalk.Component.Interop.IResourceTracker).T')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-2 'System.Func`2')

A delegate, or stream factory, that returns the stream wrapping the original one.

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.WrapOriginalDataStream_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessagePart,System.Func_System.IO.Stream,T_,Microsoft.BizTalk.Component.Interop.IResourceTracker).tracker'></a>

`tracker` [Microsoft.BizTalk.Component.Interop.IResourceTracker](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IResourceTracker 'Microsoft.BizTalk.Component.Interop.IResourceTracker')

Pipeline's resource tracker to which to report the newly created wrapping stream.

#### Returns
[T](BaseMessagePartExtensions.WrapOriginalDataStream_T_(thisIBaseMessagePart,Func_Stream,T_,IResourceTracker).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.WrapOriginalDataStream_T_(thisMicrosoft.BizTalk.Message.Interop.IBaseMessagePart,System.Func_System.IO.Stream,T_,Microsoft.BizTalk.Component.Interop.IResourceTracker).T 'Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.WrapOriginalDataStream<T>(this Microsoft.BizTalk.Message.Interop.IBaseMessagePart, System.Func<System.IO.Stream,T>, Microsoft.BizTalk.Component.Interop.IResourceTracker).T')  
The new wrapping [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') if it is not the same instance as the original one. The original [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') otherwise.