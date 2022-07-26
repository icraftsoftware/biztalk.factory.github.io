#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO')

## EnumerableStream Class

Transform an [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of either [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')s or arrays of [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')s into a
readonly, non-seekable [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') of [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')s.

```csharp
public class EnumerableStream : System.IO.Stream
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.MarshalByRefObject](https://docs.microsoft.com/en-us/dotnet/api/System.MarshalByRefObject 'System.MarshalByRefObject') &#129106; [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') &#129106; EnumerableStream

### Remarks
When [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')s are used as the underlying type of the [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1'), the [System.Text.Encoding.Unicode](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding.Unicode 'System.Text.Encoding.Unicode') encoding is assumed to convert them to [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')s.

| Constructors | |
| :--- | :--- |
| [EnumerableStream(IEnumerable&lt;byte[]&gt;)](EnumerableStream.EnumerableStream(IEnumerable_byte[]_).md 'Be.Stateless.IO.EnumerableStream.EnumerableStream(System.Collections.Generic.IEnumerable<byte[]>)') | Transform an [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of arrays of [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')s into a [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream'). |
| [EnumerableStream(IEnumerable&lt;string&gt;)](EnumerableStream.EnumerableStream(IEnumerable_string_).md 'Be.Stateless.IO.EnumerableStream.EnumerableStream(System.Collections.Generic.IEnumerable<string>)') | Transform an [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')s into a [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream'). |

| Properties | |
| :--- | :--- |
| [CanRead](EnumerableStream.CanRead.md 'Be.Stateless.IO.EnumerableStream.CanRead') | |
| [CanSeek](EnumerableStream.CanSeek.md 'Be.Stateless.IO.EnumerableStream.CanSeek') | |
| [CanWrite](EnumerableStream.CanWrite.md 'Be.Stateless.IO.EnumerableStream.CanWrite') | |
| [Length](EnumerableStream.Length.md 'Be.Stateless.IO.EnumerableStream.Length') | |
| [Position](EnumerableStream.Position.md 'Be.Stateless.IO.EnumerableStream.Position') | |

| Methods | |
| :--- | :--- |
| [Flush()](EnumerableStream.Flush().md 'Be.Stateless.IO.EnumerableStream.Flush()') | |
| [Read(byte[], int, int)](EnumerableStream.Read(byte[],int,int).md 'Be.Stateless.IO.EnumerableStream.Read(byte[], int, int)') | |
| [Seek(long, SeekOrigin)](EnumerableStream.Seek(long,SeekOrigin).md 'Be.Stateless.IO.EnumerableStream.Seek(long, System.IO.SeekOrigin)') | |
| [SetLength(long)](EnumerableStream.SetLength(long).md 'Be.Stateless.IO.EnumerableStream.SetLength(long)') | |
| [Write(byte[], int, int)](EnumerableStream.Write(byte[],int,int).md 'Be.Stateless.IO.EnumerableStream.Write(byte[], int, int)') | |
