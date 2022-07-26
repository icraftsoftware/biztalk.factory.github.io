#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream')

## CompositeXmlStream Class

Aggregates, at the stream level, several [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')s whose contents is XML.

```csharp
public class CompositeXmlStream : System.IO.Stream
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.MarshalByRefObject](https://docs.microsoft.com/en-us/dotnet/api/System.MarshalByRefObject 'System.MarshalByRefObject') &#129106; [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') &#129106; CompositeXmlStream

### Remarks

Because the input streams are aggregated at the stream level, the contents of the input streams must all be of UTF-8
encoded and cannot have an [System.Xml.XmlDeclaration](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDeclaration 'System.Xml.XmlDeclaration'). Note that it is also possible to use a
`Be.Stateless.BizTalk.Xml.CompositeXmlReader` instead of this [CompositeXmlStream](CompositeXmlStream.md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream') should you not be
able to lift either of these constraints.

The contents of the aggregated [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')s is wrapped in an XML structured as follows:

```csharp
<agg:Root xmlns:agg="http://schemas.microsoft.com/BizTalk/2003/aggschema">
              <agg:InputMessagePart_0>
                ... content of 1st message part ...
              </agg:InputMessagePart_0>
              <agg:InputMessagePart_1>
                ... content of 2nd message part ...
              </agg:InputMessagePart_1>
              ...
              <agg:InputMessagePart_n>
                ... content of nth message part ...
              </agg:InputMessagePart_n>
            </agg:Root>
```

| Constructors | |
| :--- | :--- |
| [CompositeXmlStream(Stream[])](CompositeXmlStream.CompositeXmlStream(Stream[]).md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream.CompositeXmlStream(System.IO.Stream[])') | Construct an [CompositeXmlStream](CompositeXmlStream.md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream') instance wrapper around the [streams](CompositeXmlStream.CompositeXmlStream(Stream[]).md#Be.Stateless.BizTalk.Stream.CompositeXmlStream.CompositeXmlStream(System.IO.Stream[]).streams 'Be.Stateless.BizTalk.Stream.CompositeXmlStream.CompositeXmlStream(System.IO.Stream[]).streams'). |

| Properties | |
| :--- | :--- |
| [CanRead](CompositeXmlStream.CanRead.md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream.CanRead') | When overridden in a derived class, gets a value indicating whether the current stream supports reading. |
| [CanSeek](CompositeXmlStream.CanSeek.md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream.CanSeek') | When overridden in a derived class, gets a value indicating whether the current stream supports seeking. |
| [CanWrite](CompositeXmlStream.CanWrite.md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream.CanWrite') | When overridden in a derived class, gets a value indicating whether the current stream supports writing. |
| [Length](CompositeXmlStream.Length.md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream.Length') | When overridden in a derived class, gets the length in bytes of the stream. |
| [Position](CompositeXmlStream.Position.md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream.Position') | When overridden in a derived class, gets or sets the position within the current stream. |

| Methods | |
| :--- | :--- |
| [Dispose(bool)](CompositeXmlStream.Dispose(bool).md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream.Dispose(bool)') | |
| [Flush()](CompositeXmlStream.Flush().md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream.Flush()') | When overridden in a derived class, clears all buffers for this stream and causes any buffered data to be written to the underlying device. |
| [Read(byte[], int, int)](CompositeXmlStream.Read(byte[],int,int).md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream.Read(byte[], int, int)') | When overridden in a derived class, reads a sequence of bytes from the current stream and advances the position within the stream by the number of bytes read. |
| [Seek(long, SeekOrigin)](CompositeXmlStream.Seek(long,SeekOrigin).md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream.Seek(long, System.IO.SeekOrigin)') | When overridden in a derived class, sets the position within the current stream. |
| [SetLength(long)](CompositeXmlStream.SetLength(long).md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream.SetLength(long)') | When overridden in a derived class, sets the length of the current stream. |
| [Write(byte[], int, int)](CompositeXmlStream.Write(byte[],int,int).md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream.Write(byte[], int, int)') | When overridden in a derived class, writes a sequence of bytes to the current stream and advances the current position within this stream by the number of bytes written. |
