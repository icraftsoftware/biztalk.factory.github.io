#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream').[EventingReadStream](EventingReadStream.md 'Be.Stateless.BizTalk.Stream.EventingReadStream')

## EventingReadStream.Read(byte[], int, int) Method

When overridden in a derived class, reads a sequence of bytes from the current stream and advances the position
within the stream by the number of bytes read.

```csharp
public override int Read(byte[] buffer, int offset, int count);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[],int,int).buffer'></a>

`buffer` [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

An array of bytes. When this method returns, the buffer contains the specified byte array with the values between
[offset](EventingReadStream.Read(byte[],int,int).md#Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[],int,int).offset 'Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[], int, int).offset') and ([offset](EventingReadStream.Read(byte[],int,int).md#Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[],int,int).offset 'Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[], int, int).offset') + [count](EventingReadStream.Read(byte[],int,int).md#Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[],int,int).count 'Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[], int, int).count') - 1) replaced by the bytes read
from the current source.

<a name='Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[],int,int).offset'></a>

`offset` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The zero-based byte offset in [buffer](EventingReadStream.Read(byte[],int,int).md#Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[],int,int).buffer 'Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[], int, int).buffer') at which to begin storing the data read from the current
stream.

<a name='Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[],int,int).count'></a>

`count` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The maximum number of bytes to be read from the current stream.

#### Returns
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')  
The total number of bytes read into the buffer. This can be less than the number of bytes requested if that many
bytes are not currently available, or zero (0) if the end of the stream has been reached.

#### Exceptions

[System.ArgumentNullException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentNullException 'System.ArgumentNullException')  
[buffer](EventingReadStream.Read(byte[],int,int).md#Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[],int,int).buffer 'Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[], int, int).buffer') is null.

[System.ArgumentOutOfRangeException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentOutOfRangeException 'System.ArgumentOutOfRangeException')  
[offset](EventingReadStream.Read(byte[],int,int).md#Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[],int,int).offset 'Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[], int, int).offset') or [count](EventingReadStream.Read(byte[],int,int).md#Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[],int,int).count 'Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[], int, int).count') is negative.

[System.ArgumentException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentException 'System.ArgumentException')  
The sum of [offset](EventingReadStream.Read(byte[],int,int).md#Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[],int,int).offset 'Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[], int, int).offset') and [count](EventingReadStream.Read(byte[],int,int).md#Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[],int,int).count 'Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[], int, int).count') is larger than the buffer length.

### Remarks
[Read(byte[], int, int)](EventingReadStream.Read(byte[],int,int).md 'Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[], int, int)') will always try to read as many bytes as requested to circumvent idiosyncratic clients that would
            fail to issue the required last extra call to [Read(byte[], int, int)](EventingReadStream.Read(byte[],int,int).md 'Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[], int, int)'), which would return zero (0), because that they
            assume that the end of the stream has been reached as soon as [Read(byte[], int, int)](EventingReadStream.Read(byte[],int,int).md 'Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[], int, int)') returns a total number of bytes read
            that is less than [count](EventingReadStream.Read(byte[],int,int).md#Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[],int,int).count 'Be.Stateless.BizTalk.Stream.EventingReadStream.Read(byte[], int, int).count').