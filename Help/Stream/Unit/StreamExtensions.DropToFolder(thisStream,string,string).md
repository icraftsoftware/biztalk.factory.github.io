#### [Be.Stateless.Stream.Unit](README.md 'README')
### [Be.Stateless.Unit.IO.Extensions](Be.Stateless.Unit.IO.Extensions.md 'Be.Stateless.Unit.IO.Extensions').[StreamExtensions](StreamExtensions.md 'Be.Stateless.Unit.IO.Extensions.StreamExtensions')

## StreamExtensions.DropToFolder(this Stream, string, string) Method

Save the content of a stream to disk by going through a temporary file.

```csharp
public static void DropToFolder(this System.IO.Stream stream, string folder, string name);
```
#### Parameters

<a name='Be.Stateless.Unit.IO.Extensions.StreamExtensions.DropToFolder(thisSystem.IO.Stream,string,string).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The stream whose content needs to be saved.

<a name='Be.Stateless.Unit.IO.Extensions.StreamExtensions.DropToFolder(thisSystem.IO.Stream,string,string).folder'></a>

`folder` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The folder where to save the stream.

<a name='Be.Stateless.Unit.IO.Extensions.StreamExtensions.DropToFolder(thisSystem.IO.Stream,string,string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The file name to use to save the stream.

### Remarks

The [stream](StreamExtensions.DropToFolder(thisStream,string,string).md#Be.Stateless.Unit.IO.Extensions.StreamExtensions.DropToFolder(thisSystem.IO.Stream,string,string).stream 'Be.Stateless.Unit.IO.Extensions.StreamExtensions.DropToFolder(this System.IO.Stream, string, string).stream') is first saved to a temporary file before being moved to file with the given [name](StreamExtensions.DropToFolder(thisStream,string,string).md#Be.Stateless.Unit.IO.Extensions.StreamExtensions.DropToFolder(thisSystem.IO.Stream,string,string).name 'Be.Stateless.Unit.IO.Extensions.StreamExtensions.DropToFolder(this System.IO.Stream, string, string).name'), but only after its content
has been completely flushed to disk.

The target [folder](StreamExtensions.DropToFolder(thisStream,string,string).md#Be.Stateless.Unit.IO.Extensions.StreamExtensions.DropToFolder(thisSystem.IO.Stream,string,string).folder 'Be.Stateless.Unit.IO.Extensions.StreamExtensions.DropToFolder(this System.IO.Stream, string, string).folder') is created if it does not exist.