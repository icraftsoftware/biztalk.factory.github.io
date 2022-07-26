#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream')

## ZipOutputStream Class

Wraps a zip-compressing stream around a data stream.

```csharp
public class ZipOutputStream : System.IO.Stream
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.MarshalByRefObject](https://docs.microsoft.com/en-us/dotnet/api/System.MarshalByRefObject 'System.MarshalByRefObject') &#129106; [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') &#129106; ZipOutputStream

### Remarks
[ZipOutputStream](ZipOutputStream.md 'Be.Stateless.BizTalk.Stream.ZipOutputStream') relies on [System.IO.Compression.ZipArchive](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Compression.ZipArchive 'System.IO.Compression.ZipArchive') for the compression and will have exactly one [System.IO.Compression.ZipArchiveEntry](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Compression.ZipArchiveEntry 'System.IO.Compression.ZipArchiveEntry').

### See Also
- [ZipArchive](https://docs.microsoft.com/en-us/dotnet/api/system.io.compression.ziparchive 'https://docs.microsoft.com/en-us/dotnet/api/system.io.compression.ziparchive')
- [http://my.safaribooksonline.com/book/operating-systems-and-server-administration/microsoft-biztalk/9780470046425/pipelines/121](http://my.safaribooksonline.com/book/operating-systems-and-server-administration/microsoft-biztalk/9780470046425/pipelines/121 'http://my.safaribooksonline.com/book/operating-systems-and-server-administration/microsoft-biztalk/9780470046425/pipelines/121')

| Constructors | |
| :--- | :--- |
| [ZipOutputStream(Stream, string, int)](ZipOutputStream.ZipOutputStream(Stream,string,int).md 'Be.Stateless.BizTalk.Stream.ZipOutputStream.ZipOutputStream(System.IO.Stream, string, int)') | |

| Properties | |
| :--- | :--- |
| [CanRead](ZipOutputStream.CanRead.md 'Be.Stateless.BizTalk.Stream.ZipOutputStream.CanRead') | |
| [CanSeek](ZipOutputStream.CanSeek.md 'Be.Stateless.BizTalk.Stream.ZipOutputStream.CanSeek') | |
| [CanWrite](ZipOutputStream.CanWrite.md 'Be.Stateless.BizTalk.Stream.ZipOutputStream.CanWrite') | |
| [Length](ZipOutputStream.Length.md 'Be.Stateless.BizTalk.Stream.ZipOutputStream.Length') | |
| [Position](ZipOutputStream.Position.md 'Be.Stateless.BizTalk.Stream.ZipOutputStream.Position') | |

| Methods | |
| :--- | :--- |
| [Close()](ZipOutputStream.Close().md 'Be.Stateless.BizTalk.Stream.ZipOutputStream.Close()') | |
| [Flush()](ZipOutputStream.Flush().md 'Be.Stateless.BizTalk.Stream.ZipOutputStream.Flush()') | |
| [Read(byte[], int, int)](ZipOutputStream.Read(byte[],int,int).md 'Be.Stateless.BizTalk.Stream.ZipOutputStream.Read(byte[], int, int)') | |
| [Seek(long, SeekOrigin)](ZipOutputStream.Seek(long,SeekOrigin).md 'Be.Stateless.BizTalk.Stream.ZipOutputStream.Seek(long, System.IO.SeekOrigin)') | |
| [SetLength(long)](ZipOutputStream.SetLength(long).md 'Be.Stateless.BizTalk.Stream.ZipOutputStream.SetLength(long)') | |
| [Write(byte[], int, int)](ZipOutputStream.Write(byte[],int,int).md 'Be.Stateless.BizTalk.Stream.ZipOutputStream.Write(byte[], int, int)') | |
