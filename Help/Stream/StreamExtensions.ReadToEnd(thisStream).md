#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO.Extensions](Be.Stateless.IO.Extensions.md 'Be.Stateless.IO.Extensions').[StreamExtensions](StreamExtensions.md 'Be.Stateless.IO.Extensions.StreamExtensions')

## StreamExtensions.ReadToEnd(this Stream) Method

Returns the content of the stream as a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String').

```csharp
public static string ReadToEnd(this System.IO.Stream stream);
```
#### Parameters

<a name='Be.Stateless.IO.Extensions.StreamExtensions.ReadToEnd(thisSystem.IO.Stream).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The stream whose content will be returned as a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String').

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
The [stream](StreamExtensions.ReadToEnd(thisStream).md#Be.Stateless.IO.Extensions.StreamExtensions.ReadToEnd(thisSystem.IO.Stream).stream 'Be.Stateless.IO.Extensions.StreamExtensions.ReadToEnd(this System.IO.Stream).stream')'s content as a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String').

### Remarks
The [stream](StreamExtensions.ReadToEnd(thisStream).md#Be.Stateless.IO.Extensions.StreamExtensions.ReadToEnd(thisSystem.IO.Stream).stream 'Be.Stateless.IO.Extensions.StreamExtensions.ReadToEnd(this System.IO.Stream).stream') will be rewinded before being read.