#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream')

## ReplicatingReadStream Class

A read-only [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') that replicates itself to another [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') while being
read.

```csharp
public class ReplicatingReadStream : System.IO.Stream
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.MarshalByRefObject](https://docs.microsoft.com/en-us/dotnet/api/System.MarshalByRefObject 'System.MarshalByRefObject') &#129106; [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') &#129106; ReplicatingReadStream

| Constructors | |
| :--- | :--- |
| [ReplicatingReadStream(Stream, Stream)](ReplicatingReadStream.ReplicatingReadStream(Stream,Stream).md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.ReplicatingReadStream(System.IO.Stream, System.IO.Stream)') | Construct a [ReplicatingReadStream](ReplicatingReadStream.md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream') instance. |

| Properties | |
| :--- | :--- |
| [CanRead](ReplicatingReadStream.CanRead.md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.CanRead') | When overridden in a derived class, gets a value indicating whether the current stream supports reading. |
| [CanSeek](ReplicatingReadStream.CanSeek.md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.CanSeek') | When overridden in a derived class, gets a value indicating whether the current stream supports seeking. |
| [CanWrite](ReplicatingReadStream.CanWrite.md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.CanWrite') | When overridden in a derived class, gets a value indicating whether the current stream supports writing. |
| [Length](ReplicatingReadStream.Length.md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.Length') | This property exposes the inner stream length in bytes. |
| [Position](ReplicatingReadStream.Position.md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.Position') | When overridden in a derived class, gets or sets the position within the current stream. |

| Methods | |
| :--- | :--- |
| [Dispose(bool)](ReplicatingReadStream.Dispose(bool).md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.Dispose(bool)') | |
| [Flush()](ReplicatingReadStream.Flush().md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.Flush()') | When overridden in a derived class, clears all buffers for this stream and causes any buffered data to be written to the underlying device. |
| [Read(byte[], int, int)](ReplicatingReadStream.Read(byte[],int,int).md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.Read(byte[], int, int)') | Reads and replicates a sequence of bytes from the current stream and advances the position within the stream by the number of bytes read. |
| [Seek(long, SeekOrigin)](ReplicatingReadStream.Seek(long,SeekOrigin).md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.Seek(long, System.IO.SeekOrigin)') | When overridden in a derived class, sets the position within the current stream. |
| [SetLength(long)](ReplicatingReadStream.SetLength(long).md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.SetLength(long)') | When overridden in a derived class, sets the length of the current stream. |
| [Write(byte[], int, int)](ReplicatingReadStream.Write(byte[],int,int).md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.Write(byte[], int, int)') | When overridden in a derived class, writes a sequence of bytes to the current stream and advances the current position within this stream by the number of bytes written. |
