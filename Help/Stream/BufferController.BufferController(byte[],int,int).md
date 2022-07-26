#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO').[BufferController](BufferController.md 'Be.Stateless.IO.BufferController')

## BufferController(byte[], int, int) Constructor

Wraps the `byte[]` array that need be to operated upon.

```csharp
public BufferController(byte[] buffer, int offset, int availability);
```
#### Parameters

<a name='Be.Stateless.IO.BufferController.BufferController(byte[],int,int).buffer'></a>

`buffer` [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

The underlying controlled buffer.

<a name='Be.Stateless.IO.BufferController.BufferController(byte[],int,int).offset'></a>

`offset` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The offset at which bytes can be appended to the underlying controlled buffer.

<a name='Be.Stateless.IO.BufferController.BufferController(byte[],int,int).availability'></a>

`availability` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

Number of available bytes that can be appended to the underlying controlled buffer.