#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO.Extensions](Be.Stateless.IO.Extensions.md 'Be.Stateless.IO.Extensions')

## StreamExtensions Class

```csharp
public static class StreamExtensions
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; StreamExtensions

| Methods | |
| :--- | :--- |
| [CompressToBase64String(this Stream)](StreamExtensions.CompressToBase64String(thisStream).md 'Be.Stateless.IO.Extensions.StreamExtensions.CompressToBase64String(this System.IO.Stream)') | Compress a stream and returns its compressed content as a base64 encoding. |
| [DecompressFromBase64String(this string)](StreamExtensions.DecompressFromBase64String(thisstring).md 'Be.Stateless.IO.Extensions.StreamExtensions.DecompressFromBase64String(this string)') | Decompress a base64 encoding of a compressed stream. |
| [Drain(this Stream)](StreamExtensions.Drain(thisStream).md 'Be.Stateless.IO.Extensions.StreamExtensions.Drain(this System.IO.Stream)') | Consume the content of the [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')[stream](StreamExtensions.Drain(thisStream).md#Be.Stateless.IO.Extensions.StreamExtensions.Drain(thisSystem.IO.Stream).stream 'Be.Stateless.IO.Extensions.StreamExtensions.Drain(this System.IO.Stream).stream'). |
| [GetMimeType(this Stream)](StreamExtensions.GetMimeType(thisStream).md 'Be.Stateless.IO.Extensions.StreamExtensions.GetMimeType(this System.IO.Stream)') | Determines the MIME type from the data stream provided. |
| [ReadToEnd(this Stream)](StreamExtensions.ReadToEnd(thisStream).md 'Be.Stateless.IO.Extensions.StreamExtensions.ReadToEnd(this System.IO.Stream)') | Returns the content of the stream as a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String'). |
| [Rewind(this Stream)](StreamExtensions.Rewind(thisStream).md 'Be.Stateless.IO.Extensions.StreamExtensions.Rewind(this System.IO.Stream)') | Rewind the stream to its [System.IO.Stream.Position](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream.Position 'System.IO.Stream.Position') 0. |
| [Save(this Stream, string)](StreamExtensions.Save(thisStream,string).md 'Be.Stateless.IO.Extensions.StreamExtensions.Save(this System.IO.Stream, string)') | Save the content of a stream to disk. |
| [ToBase64String(this Stream)](StreamExtensions.ToBase64String(thisStream).md 'Be.Stateless.IO.Extensions.StreamExtensions.ToBase64String(this System.IO.Stream)') | Returns a stream content as a base64 encoding. |
| [TryCompressToBase64String(this Stream, int, string)](StreamExtensions.TryCompressToBase64String(thisStream,int,string).md 'Be.Stateless.IO.Extensions.StreamExtensions.TryCompressToBase64String(this System.IO.Stream, int, string)') | Try to compress a stream and outputs its compressed content as a base64 encoded string, as long as its compressed content does not exceed a given [threshold](StreamExtensions.TryCompressToBase64String(thisStream,int,string).md#Be.Stateless.IO.Extensions.StreamExtensions.TryCompressToBase64String(thisSystem.IO.Stream,int,string).threshold 'Be.Stateless.IO.Extensions.StreamExtensions.TryCompressToBase64String(this System.IO.Stream, int, string).threshold'). Note that [threshold](StreamExtensions.TryCompressToBase64String(thisStream,int,string).md#Be.Stateless.IO.Extensions.StreamExtensions.TryCompressToBase64String(thisSystem.IO.Stream,int,string).threshold 'Be.Stateless.IO.Extensions.StreamExtensions.TryCompressToBase64String(this System.IO.Stream, int, string).threshold') is an approximate limit, and can be slightly overrun. This is because a compressing stream's length cannot be accurately determined while writing data to it. |
