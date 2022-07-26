#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO').[StringStream](StringStream.md 'Be.Stateless.IO.StringStream')

## StringStream.Read(byte[], int, int) Method

When overridden in a derived class, reads a sequence of bytes from the current stream and advances the position within
the stream by the number of bytes read.

```csharp
public override int Read(byte[] buffer, int offset, int count);
```
#### Parameters

<a name='Be.Stateless.IO.StringStream.Read(byte[],int,int).buffer'></a>

`buffer` [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

An array of bytes. When this method returns, the buffer contains the specified byte array with the values between
[offset](StringStream.Read(byte[],int,int).md#Be.Stateless.IO.StringStream.Read(byte[],int,int).offset 'Be.Stateless.IO.StringStream.Read(byte[], int, int).offset') and ([offset](StringStream.Read(byte[],int,int).md#Be.Stateless.IO.StringStream.Read(byte[],int,int).offset 'Be.Stateless.IO.StringStream.Read(byte[], int, int).offset') + [count](StringStream.Read(byte[],int,int).md#Be.Stateless.IO.StringStream.Read(byte[],int,int).count 'Be.Stateless.IO.StringStream.Read(byte[], int, int).count') - 1) replaced by the bytes read
from the current source.

<a name='Be.Stateless.IO.StringStream.Read(byte[],int,int).offset'></a>

`offset` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The zero-based byte offset in [buffer](StringStream.Read(byte[],int,int).md#Be.Stateless.IO.StringStream.Read(byte[],int,int).buffer 'Be.Stateless.IO.StringStream.Read(byte[], int, int).buffer') at which to begin storing the data read from the current
stream.

<a name='Be.Stateless.IO.StringStream.Read(byte[],int,int).count'></a>

`count` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The maximum number of bytes to be read from the current stream.

#### Returns
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')  
The total number of bytes read into the buffer. This can be less than the number of bytes requested if that many bytes
are not currently available, or zero (0) if the end of the stream has been reached.

#### Exceptions

[System.ArgumentException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentException 'System.ArgumentException')  
The sum of [offset](StringStream.Read(byte[],int,int).md#Be.Stateless.IO.StringStream.Read(byte[],int,int).offset 'Be.Stateless.IO.StringStream.Read(byte[], int, int).offset') and [count](StringStream.Read(byte[],int,int).md#Be.Stateless.IO.StringStream.Read(byte[],int,int).count 'Be.Stateless.IO.StringStream.Read(byte[], int, int).count') is larger than the buffer length.

[System.ArgumentNullException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentNullException 'System.ArgumentNullException')  
[buffer](StringStream.Read(byte[],int,int).md#Be.Stateless.IO.StringStream.Read(byte[],int,int).buffer 'Be.Stateless.IO.StringStream.Read(byte[], int, int).buffer') is null.

[System.ArgumentOutOfRangeException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentOutOfRangeException 'System.ArgumentOutOfRangeException')  
[offset](StringStream.Read(byte[],int,int).md#Be.Stateless.IO.StringStream.Read(byte[],int,int).offset 'Be.Stateless.IO.StringStream.Read(byte[], int, int).offset') or [count](StringStream.Read(byte[],int,int).md#Be.Stateless.IO.StringStream.Read(byte[],int,int).count 'Be.Stateless.IO.StringStream.Read(byte[], int, int).count') is negative.

[System.IO.IOException](https://docs.microsoft.com/en-us/dotnet/api/System.IO.IOException 'System.IO.IOException')  
An I/O error occurs.

[System.NotSupportedException](https://docs.microsoft.com/en-us/dotnet/api/System.NotSupportedException 'System.NotSupportedException')  
The stream does not support reading.

[System.ObjectDisposedException](https://docs.microsoft.com/en-us/dotnet/api/System.ObjectDisposedException 'System.ObjectDisposedException')  
Methods were called after the stream was closed.

### Remarks
The loop consists of picking up the next character from the string and extracting from it the appropriate byte by
using some simple bit manipulation. [System.BitConverter.GetBytes(System.Char)](https://docs.microsoft.com/en-us/dotnet/api/System.BitConverter.GetBytes#System_BitConverter_GetBytes_System_Char_ 'System.BitConverter.GetBytes(System.Char)') could have been used but that would
result in a 2-byte array being allocated each time the bytes for a character are retrieved, and since the whole point
of this class is to avoid extraneous allocations for large strings, that would have been a bit counterproductive.

### See Also
- [http://msdn.microsoft.com/en-us/magazine/cc163768.aspx](http://msdn.microsoft.com/en-us/magazine/cc163768.aspx 'http://msdn.microsoft.com/en-us/magazine/cc163768.aspx')