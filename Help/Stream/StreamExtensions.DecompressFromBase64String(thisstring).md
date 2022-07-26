#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO.Extensions](Be.Stateless.IO.Extensions.md 'Be.Stateless.IO.Extensions').[StreamExtensions](StreamExtensions.md 'Be.Stateless.IO.Extensions.StreamExtensions')

## StreamExtensions.DecompressFromBase64String(this string) Method

Decompress a base64 encoding of a compressed stream.

```csharp
public static System.IO.Stream DecompressFromBase64String(this string base64StringEncodedCompressedStream);
```
#### Parameters

<a name='Be.Stateless.IO.Extensions.StreamExtensions.DecompressFromBase64String(thisstring).base64StringEncodedCompressedStream'></a>

`base64StringEncodedCompressedStream` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The base64 encoding of a compressed stream.

#### Returns
[System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')  
The decoded and uncompressed stream.