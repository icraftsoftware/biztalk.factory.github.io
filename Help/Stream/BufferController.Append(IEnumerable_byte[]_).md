#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO').[BufferController](BufferController.md 'Be.Stateless.IO.BufferController')

## BufferController.Append(IEnumerable<byte[]>) Method

Append an [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of byte-array [buffers](BufferController.Append(IEnumerable_byte[]_).md#Be.Stateless.IO.BufferController.Append(System.Collections.Generic.IEnumerable_byte[]_).buffers 'Be.Stateless.IO.BufferController.Append(System.Collections.Generic.IEnumerable<byte[]>).buffers') to the underlying controlled buffer.

```csharp
public System.Collections.Generic.IEnumerable<byte[]> Append(System.Collections.Generic.IEnumerable<byte[]> buffers);
```
#### Parameters

<a name='Be.Stateless.IO.BufferController.Append(System.Collections.Generic.IEnumerable_byte[]_).buffers'></a>

`buffers` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

The [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of byte-array [buffers](BufferController.Append(IEnumerable_byte[]_).md#Be.Stateless.IO.BufferController.Append(System.Collections.Generic.IEnumerable_byte[]_).buffers 'Be.Stateless.IO.BufferController.Append(System.Collections.Generic.IEnumerable<byte[]>).buffers') to append to the underlying controlled
buffer.

#### Returns
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
The [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of byte-array buffers that could not be appended to the underlying controlled buffer
because of availability shortage. Notice that no byte will be lost, and that the first buffer in the [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of byte-array buffers might be a subset of what it was initially.