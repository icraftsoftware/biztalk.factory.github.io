#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO.Extensions](Be.Stateless.IO.Extensions.md 'Be.Stateless.IO.Extensions').[StreamExtensions](StreamExtensions.md 'Be.Stateless.IO.Extensions.StreamExtensions')

## StreamExtensions.CompressToBase64String(this Stream) Method

Compress a stream and returns its compressed content as a base64 encoding.

```csharp
public static string CompressToBase64String(this System.IO.Stream stream);
```
#### Parameters

<a name='Be.Stateless.IO.Extensions.StreamExtensions.CompressToBase64String(thisSystem.IO.Stream).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The stream to compress and encode.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
The base64 encoding of the compressed stream.