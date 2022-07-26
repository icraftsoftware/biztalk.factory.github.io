#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream')

## ReadOnlySeekableStream Class

This stream wraps an underlying stream into a read-only seekable stream. It does so by reusing BizTalk's [Microsoft.BizTalk.Streaming.ReadOnlySeekableStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.ReadOnlySeekableStream 'Microsoft.BizTalk.Streaming.ReadOnlySeekableStream') with
a [Microsoft.BizTalk.Streaming.VirtualStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.VirtualStream 'Microsoft.BizTalk.Streaming.VirtualStream').

```csharp
public class ReadOnlySeekableStream : Microsoft.BizTalk.Streaming.ReadOnlySeekableStream
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.MarshalByRefObject](https://docs.microsoft.com/en-us/dotnet/api/System.MarshalByRefObject 'System.MarshalByRefObject') &#129106; [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') &#129106; [Microsoft.BizTalk.Streaming.ReadOnlySeekableStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.ReadOnlySeekableStream 'Microsoft.BizTalk.Streaming.ReadOnlySeekableStream') &#129106; ReadOnlySeekableStream

### Remarks

The sole purpose of this Stream is to implement an often used pattern which is to use the [Microsoft.BizTalk.Streaming.ReadOnlySeekableStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.ReadOnlySeekableStream 'Microsoft.BizTalk.Streaming.ReadOnlySeekableStream') in
conjunction with a [Microsoft.BizTalk.Streaming.VirtualStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.VirtualStream 'Microsoft.BizTalk.Streaming.VirtualStream'). The pattern being that [Microsoft.BizTalk.Streaming.VirtualStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.VirtualStream 'Microsoft.BizTalk.Streaming.VirtualStream') will hold the stream
data in memory until a threshold is reached after which it will switch to disk. The benefit being that it avoids using
unnecessary IO resources for small messages. Note that there is a small performance hit once the stream changes
persistence mode.

The developer can alternatively choose to directly use the [Microsoft.BizTalk.Streaming.ReadOnlySeekableStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.ReadOnlySeekableStream 'Microsoft.BizTalk.Streaming.ReadOnlySeekableStream') which
exposes constructor forcing the stream to always store the data into a File on disk.

Note that the temporary file is created in the AppData directory of the user running the process i.e.
C:\Users\{User}\AppData\Local\Temp. For example, if the process is a BizTalk Host Instance, the temporary file will be
created in the AppData folder of the Service Account under which it is running. The temporary file name is prefixed with
the string "VST".

| Constructors | |
| :--- | :--- |
| [ReadOnlySeekableStream(Stream, int, int)](ReadOnlySeekableStream.ReadOnlySeekableStream(Stream,int,int).md 'Be.Stateless.BizTalk.Stream.ReadOnlySeekableStream.ReadOnlySeekableStream(System.IO.Stream, int, int)') | Constructor. |
