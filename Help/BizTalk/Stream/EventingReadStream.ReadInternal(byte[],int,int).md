#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream').[EventingReadStream](EventingReadStream.md 'Be.Stateless.BizTalk.Stream.EventingReadStream')

## EventingReadStream.ReadInternal(byte[], int, int) Method

Delegates to [InnerStream](EventingReadStream.InnerStream.md 'Be.Stateless.BizTalk.Stream.EventingReadStream.InnerStream').

```csharp
protected override int ReadInternal(byte[] buffer, int offset, int count);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Stream.EventingReadStream.ReadInternal(byte[],int,int).buffer'></a>

`buffer` [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

An array of bytes. When this method returns, the buffer contains the specified byte array with the values between
[offset](EventingReadStream.ReadInternal(byte[],int,int).md#Be.Stateless.BizTalk.Stream.EventingReadStream.ReadInternal(byte[],int,int).offset 'Be.Stateless.BizTalk.Stream.EventingReadStream.ReadInternal(byte[], int, int).offset') and ([offset](EventingReadStream.ReadInternal(byte[],int,int).md#Be.Stateless.BizTalk.Stream.EventingReadStream.ReadInternal(byte[],int,int).offset 'Be.Stateless.BizTalk.Stream.EventingReadStream.ReadInternal(byte[], int, int).offset') + [count](EventingReadStream.ReadInternal(byte[],int,int).md#Be.Stateless.BizTalk.Stream.EventingReadStream.ReadInternal(byte[],int,int).count 'Be.Stateless.BizTalk.Stream.EventingReadStream.ReadInternal(byte[], int, int).count') - 1) replaced by the bytes read
from the current source.

<a name='Be.Stateless.BizTalk.Stream.EventingReadStream.ReadInternal(byte[],int,int).offset'></a>

`offset` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The zero-based byte offset in [buffer](EventingReadStream.ReadInternal(byte[],int,int).md#Be.Stateless.BizTalk.Stream.EventingReadStream.ReadInternal(byte[],int,int).buffer 'Be.Stateless.BizTalk.Stream.EventingReadStream.ReadInternal(byte[], int, int).buffer') at which to begin storing the data read from the current
stream.

<a name='Be.Stateless.BizTalk.Stream.EventingReadStream.ReadInternal(byte[],int,int).count'></a>

`count` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The maximum number of bytes to be read from the current stream.

#### Returns
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')  
The total number of bytes read into the buffer.