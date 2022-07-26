#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO').[BufferController](BufferController.md 'Be.Stateless.IO.BufferController')

## BufferController.Append(byte[]) Method

Append an array of bytes to the underlying controlled buffer.

```csharp
public byte[] Append(byte[] bytes);
```
#### Parameters

<a name='Be.Stateless.IO.BufferController.Append(byte[]).bytes'></a>

`bytes` [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

The array of bytes to append.

#### Returns
[System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')  
The [bytes](BufferController.Append(byte[]).md#Be.Stateless.IO.BufferController.Append(byte[]).bytes 'Be.Stateless.IO.BufferController.Append(byte[]).bytes') sub-array, that is the array of bytes, that could not be appended to the underlying
controlled buffer because of availability shortage.