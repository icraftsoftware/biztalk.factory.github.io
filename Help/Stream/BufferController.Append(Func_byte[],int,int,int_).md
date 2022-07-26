#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO').[BufferController](BufferController.md 'Be.Stateless.IO.BufferController')

## BufferController.Append(Func<byte[],int,int,int>) Method

Append to the underlying buffer by delegation.

```csharp
public int Append(System.Func<byte[],int,int,int> @delegate);
```
#### Parameters

<a name='Be.Stateless.IO.BufferController.Append(System.Func_byte[],int,int,int_).delegate'></a>

`delegate` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-4 'System.Func`4')[System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-4 'System.Func`4')[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-4 'System.Func`4')[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Func-4 'System.Func`4')[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-4 'System.Func`4')

A [System.Func&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1') delegate with both a signature and semantics identical to the one of the [System.IO.Stream.Read(System.Byte[],System.Int32,System.Int32)](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream.Read#System_IO_Stream_Read_System_Byte[],System_Int32,System_Int32_ 'System.IO.Stream.Read(System.Byte[],System.Int32,System.Int32)') method.

#### Returns
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')  
The total number of bytes appended to the underlying controlled buffer.