#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO.Extensions](Be.Stateless.IO.Extensions.md 'Be.Stateless.IO.Extensions').[StreamExtensions](StreamExtensions.md 'Be.Stateless.IO.Extensions.StreamExtensions')

## StreamExtensions.Drain(this Stream) Method

Consume the content of the [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')[stream](StreamExtensions.Drain(thisStream).md#Be.Stateless.IO.Extensions.StreamExtensions.Drain(thisSystem.IO.Stream).stream 'Be.Stateless.IO.Extensions.StreamExtensions.Drain(this System.IO.Stream).stream').

```csharp
public static void Drain(this System.IO.Stream stream);
```
#### Parameters

<a name='Be.Stateless.IO.Extensions.StreamExtensions.Drain(thisSystem.IO.Stream).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The stream to drain.

### Remarks
The position of the [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')[stream](StreamExtensions.Drain(thisStream).md#Be.Stateless.IO.Extensions.StreamExtensions.Drain(thisSystem.IO.Stream).stream 'Be.Stateless.IO.Extensions.StreamExtensions.Drain(this System.IO.Stream).stream') will be moved to the end of stream.