#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream').[ReplicatingReadStream](ReplicatingReadStream.md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream')

## ReplicatingReadStream.Write(byte[], int, int) Method

When overridden in a derived class, writes a sequence of bytes to the current stream and advances the current
position within this stream by the number of bytes written.

```csharp
public override void Write(byte[] buffer, int offset, int count);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Stream.ReplicatingReadStream.Write(byte[],int,int).buffer'></a>

`buffer` [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

An array of bytes. This method copies count bytes from [buffer](ReplicatingReadStream.Write(byte[],int,int).md#Be.Stateless.BizTalk.Stream.ReplicatingReadStream.Write(byte[],int,int).buffer 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.Write(byte[], int, int).buffer') to the current stream.

<a name='Be.Stateless.BizTalk.Stream.ReplicatingReadStream.Write(byte[],int,int).offset'></a>

`offset` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The zero-based byte offset in [buffer](ReplicatingReadStream.Write(byte[],int,int).md#Be.Stateless.BizTalk.Stream.ReplicatingReadStream.Write(byte[],int,int).buffer 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream.Write(byte[], int, int).buffer') at which to begin copying bytes to the current stream.

<a name='Be.Stateless.BizTalk.Stream.ReplicatingReadStream.Write(byte[],int,int).count'></a>

`count` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The number of bytes to be written to the current stream.

#### Exceptions

[System.NotSupportedException](https://docs.microsoft.com/en-us/dotnet/api/System.NotSupportedException 'System.NotSupportedException')  
The stream does not support writing.