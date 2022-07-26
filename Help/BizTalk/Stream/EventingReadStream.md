#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream')

## EventingReadStream Class

An eventing read-only stream replacement of [Microsoft.BizTalk.Streaming.EventingReadStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.EventingReadStream 'Microsoft.BizTalk.Streaming.EventingReadStream') that
deterministically fires the [Microsoft.BizTalk.Streaming.IProvideReadStreamEvents.AfterLastReadEvent](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.IProvideReadStreamEvents.AfterLastReadEvent 'Microsoft.BizTalk.Streaming.IProvideReadStreamEvents.AfterLastReadEvent') event.

```csharp
public class EventingReadStream : Microsoft.BizTalk.Streaming.EventingReadStream
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.MarshalByRefObject](https://docs.microsoft.com/en-us/dotnet/api/System.MarshalByRefObject 'System.MarshalByRefObject') &#129106; [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') &#129106; [Microsoft.BizTalk.Streaming.EventingReadStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.EventingReadStream 'Microsoft.BizTalk.Streaming.EventingReadStream') &#129106; EventingReadStream

### Remarks

In short terms, this stream ensures that its contents is always exhausted and end-of-stream detection happens
deterministically.

In detailed terms, regardless of whether this stream's client will assume the end-of-stream has been reached as soon as
a [System.IO.Stream.Read(System.Byte[],System.Int32,System.Int32)](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream.Read#System_IO_Stream_Read_System_Byte[],System_Int32,System_Int32_ 'System.IO.Stream.Read(System.Byte[],System.Int32,System.Int32)') operation returns less bytes than the number of bytes requested, or whether it
will only assume the end-of-stream has been reached once the [System.IO.Stream.Read(System.Byte[],System.Int32,System.Int32)](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream.Read#System_IO_Stream_Read_System_Byte[],System_Int32,System_Int32_ 'System.IO.Stream.Read(System.Byte[],System.Int32,System.Int32)') operation returns zero
(0) — which is, by the way, the officially documented way of being notified the end-of-stream has been reached
— an [EventingReadStream](EventingReadStream.md 'Be.Stateless.BizTalk.Stream.EventingReadStream') instance will always fire the [Microsoft.BizTalk.Streaming.IProvideReadStreamEvents.AfterLastReadEvent](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.IProvideReadStreamEvents.AfterLastReadEvent 'Microsoft.BizTalk.Streaming.IProvideReadStreamEvents.AfterLastReadEvent') event as soon as the inner stream's end has been reached.

| Constructors | |
| :--- | :--- |
| [EventingReadStream(Stream)](EventingReadStream.EventingReadStream(Stream).md 'Be.Stateless.BizTalk.Stream.EventingReadStream.EventingReadStream(System.IO.Stream)') | Construct an [EventingReadStream](EventingReadStream.md 'Be.Stateless.BizTalk.Stream.EventingReadStream') instance wrapper around [stream](EventingReadStream.EventingReadStream(Stream).md#Be.Stateless.BizTalk.Stream.EventingReadStream.EventingReadStream(System.IO.Stream).stream 'Be.Stateless.BizTalk.Stream.EventingReadStream.EventingReadStream(System.IO.Stream).stream'). |

| Properties | |
| :--- | :--- |
| [CanRead](EventingReadStream.CanRead.md 'Be.Stateless.BizTalk.Stream.EventingReadStream.CanRead') | When overridden in a derived class, gets a value indicating whether the current stream supports reading. |
| [CanSeek](EventingReadStream.CanSeek.md 'Be.Stateless.BizTalk.Stream.EventingReadStream.CanSeek') | When overridden in a derived class, gets a value indicating whether the current stream supports seeking. |
| [InnerStream](EventingReadStream.InnerStream.md 'Be.Stateless.BizTalk.Stream.EventingReadStream.InnerStream') | The wrapped inner [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream'). |
| [Length](EventingReadStream.Length.md 'Be.Stateless.BizTalk.Stream.EventingReadStream.Length') | This property returns the inner stream length in bytes. |
| [Position](EventingReadStream.Position.md 'Be.Stateless.BizTalk.Stream.EventingReadStream.Position') | When overridden in a derived class, gets or sets the position within the current stream. |

| Methods | |
| :--- | :--- |
| [Dispose(bool)](EventingReadStream.Dispose(bool).md 'Be.Stateless.BizTalk.Stream.EventingReadStream.Dispose(bool)') | |
| [Flush()](EventingReadStream.Flush().md 'Be.Stateless.BizTalk.Stream.EventingReadStream.Flush()') | When overridden in a derived class, clears all buffers for this stream and causes any buffered data to be written to the underlying device. |
| [Read(byte[], int, int)](EventingReadStream.Read(byte[],int,int).md 'Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[], int, int)') | When overridden in a derived class, reads a sequence of bytes from the current stream and advances the position within the stream by the number of bytes read. |
| [ReadInternal(byte[], int, int)](EventingReadStream.ReadInternal(byte[],int,int).md 'Be.Stateless.BizTalk.Stream.EventingReadStream.ReadInternal(byte[], int, int)') | Delegates to [InnerStream](EventingReadStream.InnerStream.md 'Be.Stateless.BizTalk.Stream.EventingReadStream.InnerStream'). |
| [Seek(long, SeekOrigin)](EventingReadStream.Seek(long,SeekOrigin).md 'Be.Stateless.BizTalk.Stream.EventingReadStream.Seek(long, System.IO.SeekOrigin)') | When overridden in a derived class, sets the position within the current stream. |
| [SetLength(long)](EventingReadStream.SetLength(long).md 'Be.Stateless.BizTalk.Stream.EventingReadStream.SetLength(long)') | When overridden in a derived class, sets the length of the current stream. |
| [ThrowIfDisposed()](EventingReadStream.ThrowIfDisposed().md 'Be.Stateless.BizTalk.Stream.EventingReadStream.ThrowIfDisposed()') | |
