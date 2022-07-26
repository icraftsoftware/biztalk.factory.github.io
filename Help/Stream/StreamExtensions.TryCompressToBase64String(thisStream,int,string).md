#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO.Extensions](Be.Stateless.IO.Extensions.md 'Be.Stateless.IO.Extensions').[StreamExtensions](StreamExtensions.md 'Be.Stateless.IO.Extensions.StreamExtensions')

## StreamExtensions.TryCompressToBase64String(this Stream, int, string) Method

Try to compress a stream and outputs its compressed content as a base64 encoded string, as long as its compressed content does not exceed a given [threshold](StreamExtensions.TryCompressToBase64String(thisStream,int,string).md#Be.Stateless.IO.Extensions.StreamExtensions.TryCompressToBase64String(thisSystem.IO.Stream,int,string).threshold 'Be.Stateless.IO.Extensions.StreamExtensions.TryCompressToBase64String(this System.IO.Stream, int, string).threshold'). Note that [threshold](StreamExtensions.TryCompressToBase64String(thisStream,int,string).md#Be.Stateless.IO.Extensions.StreamExtensions.TryCompressToBase64String(thisSystem.IO.Stream,int,string).threshold 'Be.Stateless.IO.Extensions.StreamExtensions.TryCompressToBase64String(this System.IO.Stream, int, string).threshold') is an approximate limit, and can be slightly overrun. This is because a compressing stream's length
cannot be accurately determined while writing data to it.

```csharp
public static bool TryCompressToBase64String(this System.IO.Stream stream, int threshold, out string compressedBase64String);
```
#### Parameters

<a name='Be.Stateless.IO.Extensions.StreamExtensions.TryCompressToBase64String(thisSystem.IO.Stream,int,string).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The stream to compress and encode.

<a name='Be.Stateless.IO.Extensions.StreamExtensions.TryCompressToBase64String(thisSystem.IO.Stream,int,string).threshold'></a>

`threshold` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The threshold in bytes that the compressed stream cannot exceed. Notice that this threshold is approximate, and can in certain cases be exceeded.

<a name='Be.Stateless.IO.Extensions.StreamExtensions.TryCompressToBase64String(thisSystem.IO.Stream,int,string).compressedBase64String'></a>

`compressedBase64String` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The base64 encoding of the compressed stream if the latter's length does not exceed the compression threshold.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if the stream can be compressed without exceeding the [threshold](StreamExtensions.TryCompressToBase64String(thisStream,int,string).md#Be.Stateless.IO.Extensions.StreamExtensions.TryCompressToBase64String(thisSystem.IO.Stream,int,string).threshold 'Be.Stateless.IO.Extensions.StreamExtensions.TryCompressToBase64String(this System.IO.Stream, int, string).threshold'); `false`
            otherwise.