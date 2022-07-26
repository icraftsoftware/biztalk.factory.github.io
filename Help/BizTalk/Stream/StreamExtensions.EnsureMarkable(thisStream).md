#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream.Extensions](Be.Stateless.BizTalk.Stream.Extensions.md 'Be.Stateless.BizTalk.Stream.Extensions').[StreamExtensions](StreamExtensions.md 'Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions')

## StreamExtensions.EnsureMarkable(this Stream) Method

Ensure the [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') is wrapped in a [Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream 'Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream') and
thereby ready for probing, see [Probe(this Stream)](StreamExtensions.Probe(thisStream).md 'Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions.Probe(this System.IO.Stream)').

```csharp
public static Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream EnsureMarkable(this System.IO.Stream stream);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions.EnsureMarkable(thisSystem.IO.Stream).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The current [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream').

#### Returns
[Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream 'Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream')  
A [Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream 'Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream') stream.

#### Exceptions

[System.InvalidCastException](https://docs.microsoft.com/en-us/dotnet/api/System.InvalidCastException 'System.InvalidCastException')  
If [stream](StreamExtensions.EnsureMarkable(thisStream).md#Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions.EnsureMarkable(thisSystem.IO.Stream).stream 'Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions.EnsureMarkable(this System.IO.Stream).stream') is not already wrapped in a [Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream 'Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream').