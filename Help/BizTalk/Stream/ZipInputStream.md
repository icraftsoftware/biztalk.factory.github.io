#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream')

## ZipInputStream Class

Wraps a zip-decompressing stream around a data stream and ensures that the data stream is exhausted once the
decompression is complete. It supports the PK Zip archive format with an entry compressed with the DEFLATE algorithm.

```csharp
public class ZipInputStream : System.IO.Stream
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.MarshalByRefObject](https://docs.microsoft.com/en-us/dotnet/api/System.MarshalByRefObject 'System.MarshalByRefObject') &#129106; [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') &#129106; ZipInputStream

### Remarks
[ZipInputStream](ZipInputStream.md 'Be.Stateless.BizTalk.Stream.ZipInputStream') relies on [System.IO.Compression.ZipArchive](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Compression.ZipArchive 'System.IO.Compression.ZipArchive') for the decompression of the zip-stream. The stream
            containing the zipped data must have exactly one [System.IO.Compression.ZipArchiveEntry](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Compression.ZipArchiveEntry 'System.IO.Compression.ZipArchiveEntry'). If more than one entry exist, only the
            first one is decompressed and the remaining entries are disregarded. If the underlying stream given to the constructor
            is not seekable, [ZipInputStream](ZipInputStream.md 'Be.Stateless.BizTalk.Stream.ZipInputStream') will leverage [ReadOnlySeekableStream](ReadOnlySeekableStream.md 'Be.Stateless.BizTalk.Stream.ReadOnlySeekableStream') to avoid loading the
            whole stream in memory. This is necessary as [System.IO.Compression.ZipArchive](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Compression.ZipArchive 'System.IO.Compression.ZipArchive') loads the entire archive stream in memory if the
            underlying stream does not support seeking.

### See Also
- [ZipArchive](https://docs.microsoft.com/en-us/dotnet/api/system.io.compression.ziparchive 'https://docs.microsoft.com/en-us/dotnet/api/system.io.compression.ziparchive')
- [ZipArchiveMode](https://docs.microsoft.com/en-us/dotnet/api/system.io.compression.ziparchivemode#remarks 'https://docs.microsoft.com/en-us/dotnet/api/system.io.compression.ziparchivemode#remarks')

| Constructors | |
| :--- | :--- |
| [ZipInputStream(Stream)](ZipInputStream.ZipInputStream(Stream).md 'Be.Stateless.BizTalk.Stream.ZipInputStream.ZipInputStream(System.IO.Stream)') | |

| Properties | |
| :--- | :--- |
| [CanRead](ZipInputStream.CanRead.md 'Be.Stateless.BizTalk.Stream.ZipInputStream.CanRead') | |
| [CanSeek](ZipInputStream.CanSeek.md 'Be.Stateless.BizTalk.Stream.ZipInputStream.CanSeek') | |
| [CanWrite](ZipInputStream.CanWrite.md 'Be.Stateless.BizTalk.Stream.ZipInputStream.CanWrite') | |
| [Length](ZipInputStream.Length.md 'Be.Stateless.BizTalk.Stream.ZipInputStream.Length') | |
| [Position](ZipInputStream.Position.md 'Be.Stateless.BizTalk.Stream.ZipInputStream.Position') | |

| Methods | |
| :--- | :--- |
| [Close()](ZipInputStream.Close().md 'Be.Stateless.BizTalk.Stream.ZipInputStream.Close()') | |
| [Flush()](ZipInputStream.Flush().md 'Be.Stateless.BizTalk.Stream.ZipInputStream.Flush()') | |
| [Read(byte[], int, int)](ZipInputStream.Read(byte[],int,int).md 'Be.Stateless.BizTalk.Stream.ZipInputStream.Read(byte[], int, int)') | |
| [Seek(long, SeekOrigin)](ZipInputStream.Seek(long,SeekOrigin).md 'Be.Stateless.BizTalk.Stream.ZipInputStream.Seek(long, System.IO.SeekOrigin)') | |
| [SetLength(long)](ZipInputStream.SetLength(long).md 'Be.Stateless.BizTalk.Stream.ZipInputStream.SetLength(long)') | |
| [Write(byte[], int, int)](ZipInputStream.Write(byte[],int,int).md 'Be.Stateless.BizTalk.Stream.ZipInputStream.Write(byte[], int, int)') | |
