#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream.Extensions](Be.Stateless.BizTalk.Stream.Extensions.md 'Be.Stateless.BizTalk.Stream.Extensions').[StreamExtensions](StreamExtensions.md 'Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions')

## StreamExtensions.Probe(this Stream) Method

Support for [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') probing.

```csharp
public static Be.Stateless.BizTalk.Stream.Extensions.IProbeStream Probe(this System.IO.Stream stream);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions.Probe(thisSystem.IO.Stream).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The current [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream').

#### Returns
[IProbeStream](IProbeStream.md 'Be.Stateless.BizTalk.Stream.Extensions.IProbeStream')  
The [IProbeStream](IProbeStream.md 'Be.Stateless.BizTalk.Stream.Extensions.IProbeStream') instance that will probe the current [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')s.

### Remarks
The [stream](StreamExtensions.Probe(thisStream).md#Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions.Probe(thisSystem.IO.Stream).stream 'Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions.Probe(this System.IO.Stream).stream') is expected to be markable, that is to say, it has to be of type [Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream 'Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream').