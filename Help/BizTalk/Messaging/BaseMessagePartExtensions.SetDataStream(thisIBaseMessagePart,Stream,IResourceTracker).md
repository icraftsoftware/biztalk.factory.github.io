#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Message.Extensions](Be.Stateless.BizTalk.Message.Extensions.md 'Be.Stateless.BizTalk.Message.Extensions').[BaseMessagePartExtensions](BaseMessagePartExtensions.md 'Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions')

## BaseMessagePartExtensions.SetDataStream(this IBaseMessagePart, Stream, IResourceTracker) Method

Replaces this [messagePart](BaseMessagePartExtensions.SetDataStream(thisIBaseMessagePart,Stream,IResourceTracker).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.SetDataStream(thisMicrosoft.BizTalk.Message.Interop.IBaseMessagePart,System.IO.Stream,Microsoft.BizTalk.Component.Interop.IResourceTracker).messagePart 'Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.SetDataStream(this Microsoft.BizTalk.Message.Interop.IBaseMessagePart, System.IO.Stream, Microsoft.BizTalk.Component.Interop.IResourceTracker).messagePart')'s original data stream by another [stream](BaseMessagePartExtensions.SetDataStream(thisIBaseMessagePart,Stream,IResourceTracker).md#Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.SetDataStream(thisMicrosoft.BizTalk.Message.Interop.IBaseMessagePart,System.IO.Stream,Microsoft.BizTalk.Component.Interop.IResourceTracker).stream 'Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.SetDataStream(this Microsoft.BizTalk.Message.Interop.IBaseMessagePart, System.IO.Stream, Microsoft.BizTalk.Component.Interop.IResourceTracker).stream').

```csharp
public static void SetDataStream(this Microsoft.BizTalk.Message.Interop.IBaseMessagePart messagePart, System.IO.Stream stream, Microsoft.BizTalk.Component.Interop.IResourceTracker tracker);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.SetDataStream(thisMicrosoft.BizTalk.Message.Interop.IBaseMessagePart,System.IO.Stream,Microsoft.BizTalk.Component.Interop.IResourceTracker).messagePart'></a>

`messagePart` [Microsoft.BizTalk.Message.Interop.IBaseMessagePart](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessagePart 'Microsoft.BizTalk.Message.Interop.IBaseMessagePart')

The part whose original data stream is replaced.

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.SetDataStream(thisMicrosoft.BizTalk.Message.Interop.IBaseMessagePart,System.IO.Stream,Microsoft.BizTalk.Component.Interop.IResourceTracker).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The replacement stream.

<a name='Be.Stateless.BizTalk.Message.Extensions.BaseMessagePartExtensions.SetDataStream(thisMicrosoft.BizTalk.Message.Interop.IBaseMessagePart,System.IO.Stream,Microsoft.BizTalk.Component.Interop.IResourceTracker).tracker'></a>

`tracker` [Microsoft.BizTalk.Component.Interop.IResourceTracker](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IResourceTracker 'Microsoft.BizTalk.Component.Interop.IResourceTracker')

Pipeline's resource tracker to which to report the newly created wrapping stream.