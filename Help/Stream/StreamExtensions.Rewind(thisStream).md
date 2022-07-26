#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO.Extensions](Be.Stateless.IO.Extensions.md 'Be.Stateless.IO.Extensions').[StreamExtensions](StreamExtensions.md 'Be.Stateless.IO.Extensions.StreamExtensions')

## StreamExtensions.Rewind(this Stream) Method

Rewind the stream to its [System.IO.Stream.Position](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream.Position 'System.IO.Stream.Position') 0.

```csharp
public static System.IO.Stream Rewind(this System.IO.Stream stream);
```
#### Parameters

<a name='Be.Stateless.IO.Extensions.StreamExtensions.Rewind(thisSystem.IO.Stream).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') to rewind.

#### Returns
[System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')  
The [stream](StreamExtensions.Rewind(thisStream).md#Be.Stateless.IO.Extensions.StreamExtensions.Rewind(thisSystem.IO.Stream).stream 'Be.Stateless.IO.Extensions.StreamExtensions.Rewind(this System.IO.Stream).stream') which has been rewinded.

#### Exceptions

[System.InvalidOperationException](https://docs.microsoft.com/en-us/dotnet/api/System.InvalidOperationException 'System.InvalidOperationException')  
If the [stream](StreamExtensions.Rewind(thisStream).md#Be.Stateless.IO.Extensions.StreamExtensions.Rewind(thisSystem.IO.Stream).stream 'Be.Stateless.IO.Extensions.StreamExtensions.Rewind(this System.IO.Stream).stream') is not seekable, i.e. [System.IO.Stream.CanSeek](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream.CanSeek 'System.IO.Stream.CanSeek') is `false`.