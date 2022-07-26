#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO').[BufferController](BufferController.md 'Be.Stateless.IO.BufferController')

## BufferController.Append(byte[], int, int) Method

Append a sequence of bytes from the given [bytes](BufferController.Append(byte[],int,int).md#Be.Stateless.IO.BufferController.Append(byte[],int,int).bytes 'Be.Stateless.IO.BufferController.Append(byte[], int, int).bytes') array to the underlying controlled buffer.

```csharp
public byte[] Append(byte[] bytes, int offset, int count);
```
#### Parameters

<a name='Be.Stateless.IO.BufferController.Append(byte[],int,int).bytes'></a>

`bytes` [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

An array of bytes. This method appends count bytes from [bytes](BufferController.Append(byte[],int,int).md#Be.Stateless.IO.BufferController.Append(byte[],int,int).bytes 'Be.Stateless.IO.BufferController.Append(byte[], int, int).bytes') to the underlying controlled buffer.

<a name='Be.Stateless.IO.BufferController.Append(byte[],int,int).offset'></a>

`offset` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The zero-based byte offset in [bytes](BufferController.Append(byte[],int,int).md#Be.Stateless.IO.BufferController.Append(byte[],int,int).bytes 'Be.Stateless.IO.BufferController.Append(byte[], int, int).bytes') at which to begin copying bytes to the underlying controlled
buffer.

<a name='Be.Stateless.IO.BufferController.Append(byte[],int,int).count'></a>

`count` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The number of bytes to be written to the underlying controlled buffer.

#### Returns
[System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')  
The [bytes](BufferController.Append(byte[],int,int).md#Be.Stateless.IO.BufferController.Append(byte[],int,int).bytes 'Be.Stateless.IO.BufferController.Append(byte[], int, int).bytes') sub-array, that is the array of bytes, that could not be appended to the underlying
controlled buffer because of availability shortage.

#### Exceptions

[System.ArgumentNullException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentNullException 'System.ArgumentNullException')  
[bytes](BufferController.Append(byte[],int,int).md#Be.Stateless.IO.BufferController.Append(byte[],int,int).bytes 'Be.Stateless.IO.BufferController.Append(byte[], int, int).bytes') is null.

[System.ArgumentOutOfRangeException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentOutOfRangeException 'System.ArgumentOutOfRangeException')  
[offset](BufferController.Append(byte[],int,int).md#Be.Stateless.IO.BufferController.Append(byte[],int,int).offset 'Be.Stateless.IO.BufferController.Append(byte[], int, int).offset') or [count](BufferController.Append(byte[],int,int).md#Be.Stateless.IO.BufferController.Append(byte[],int,int).count 'Be.Stateless.IO.BufferController.Append(byte[], int, int).count') is negative.

[System.ArgumentException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentException 'System.ArgumentException')  
The sum of [offset](BufferController.Append(byte[],int,int).md#Be.Stateless.IO.BufferController.Append(byte[],int,int).offset 'Be.Stateless.IO.BufferController.Append(byte[], int, int).offset') and [count](BufferController.Append(byte[],int,int).md#Be.Stateless.IO.BufferController.Append(byte[],int,int).count 'Be.Stateless.IO.BufferController.Append(byte[], int, int).count') is greater than the [bytes](BufferController.Append(byte[],int,int).md#Be.Stateless.IO.BufferController.Append(byte[],int,int).bytes 'Be.Stateless.IO.BufferController.Append(byte[], int, int).bytes')' array
length.