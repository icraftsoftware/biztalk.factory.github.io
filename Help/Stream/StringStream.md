#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO')

## StringStream Class

Stream-derived class meant to minimize the amount of overhead required to wrap a string as a stream.

```csharp
public class StringStream : System.IO.Stream
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.MarshalByRefObject](https://docs.microsoft.com/en-us/dotnet/api/System.MarshalByRefObject 'System.MarshalByRefObject') &#129106; [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') &#129106; StringStream

### Remarks

Notice that a Unicode BOM (see [System.Text.Encoding.GetPreamble](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding.GetPreamble 'System.Text.Encoding.GetPreamble')), is always inserted at the beginning of the [StringStream](StringStream.md 'Be.Stateless.IO.StringStream')'s content.

### See Also
- [http://msdn.microsoft.com/en-us/magazine/cc163768.aspx](http://msdn.microsoft.com/en-us/magazine/cc163768.aspx 'http://msdn.microsoft.com/en-us/magazine/cc163768.aspx')

| Constructors | |
| :--- | :--- |
| [StringStream(string)](StringStream.StringStream(string).md 'Be.Stateless.IO.StringStream.StringStream(string)') | Instantiate a new [StringStream](StringStream.md 'Be.Stateless.IO.StringStream') that wraps a given [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String'). |

| Properties | |
| :--- | :--- |
| [CanRead](StringStream.CanRead.md 'Be.Stateless.IO.StringStream.CanRead') | |
| [CanSeek](StringStream.CanSeek.md 'Be.Stateless.IO.StringStream.CanSeek') | |
| [CanWrite](StringStream.CanWrite.md 'Be.Stateless.IO.StringStream.CanWrite') | |
| [Length](StringStream.Length.md 'Be.Stateless.IO.StringStream.Length') | When overridden in a derived class, gets the length in bytes of the stream. |
| [Position](StringStream.Position.md 'Be.Stateless.IO.StringStream.Position') | |

| Methods | |
| :--- | :--- |
| [Flush()](StringStream.Flush().md 'Be.Stateless.IO.StringStream.Flush()') | |
| [Read(byte[], int, int)](StringStream.Read(byte[],int,int).md 'Be.Stateless.IO.StringStream.Read(byte[], int, int)') | When overridden in a derived class, reads a sequence of bytes from the current stream and advances the position within the stream by the number of bytes read. |
| [Seek(long, SeekOrigin)](StringStream.Seek(long,SeekOrigin).md 'Be.Stateless.IO.StringStream.Seek(long, System.IO.SeekOrigin)') | |
| [SetLength(long)](StringStream.SetLength(long).md 'Be.Stateless.IO.StringStream.SetLength(long)') | |
| [Write(byte[], int, int)](StringStream.Write(byte[],int,int).md 'Be.Stateless.IO.StringStream.Write(byte[], int, int)') | |
