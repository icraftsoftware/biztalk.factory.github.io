#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream').[ReadOnlySeekableStream](ReadOnlySeekableStream.md 'Be.Stateless.BizTalk.Stream.ReadOnlySeekableStream')

## ReadOnlySeekableStream(Stream, int, int) Constructor

Constructor.

```csharp
public ReadOnlySeekableStream(System.IO.Stream source, int bufferSize=8192, int thresholdSize=1048576);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Stream.ReadOnlySeekableStream.ReadOnlySeekableStream(System.IO.Stream,int,int).source'></a>

`source` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The underlying stream.

<a name='Be.Stateless.BizTalk.Stream.ReadOnlySeekableStream.ReadOnlySeekableStream(System.IO.Stream,int,int).bufferSize'></a>

`bufferSize` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

Buffer size in bytes used by [Microsoft.BizTalk.Streaming.ReadOnlySeekableStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.ReadOnlySeekableStream 'Microsoft.BizTalk.Streaming.ReadOnlySeekableStream') and [Microsoft.BizTalk.Streaming.VirtualStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.VirtualStream 'Microsoft.BizTalk.Streaming.VirtualStream').

<a name='Be.Stateless.BizTalk.Stream.ReadOnlySeekableStream.ReadOnlySeekableStream(System.IO.Stream,int,int).thresholdSize'></a>

`thresholdSize` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

Size in bytes after which [Microsoft.BizTalk.Streaming.VirtualStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.VirtualStream 'Microsoft.BizTalk.Streaming.VirtualStream') will switch from a MemoryStream to a FileStream.