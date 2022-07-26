#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO')

## BufferController Class

Control operations on a temporary buffer.

```csharp
public class BufferController
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; BufferController

### Remarks
A temporary buffer is typically used in a [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')-based component while reading from one [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') and writing to an other, or when one needs to transcode the bytes that have been read before being
written to the buffer allocated by the [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')'s client.

| Constructors | |
| :--- | :--- |
| [BufferController(byte[], int, int)](BufferController.BufferController(byte[],int,int).md 'Be.Stateless.IO.BufferController.BufferController(byte[], int, int)') | Wraps the `byte[]` array that need be to operated upon. |

| Properties | |
| :--- | :--- |
| [Availability](BufferController.Availability.md 'Be.Stateless.IO.BufferController.Availability') | The number of available bytes than have yet to be appended to the underlying controlled buffer. |
| [Count](BufferController.Count.md 'Be.Stateless.IO.BufferController.Count') | The total number of bytes that have been appended to the underlying controlled buffer. |

| Methods | |
| :--- | :--- |
| [Append(byte[], int, int)](BufferController.Append(byte[],int,int).md 'Be.Stateless.IO.BufferController.Append(byte[], int, int)') | Append a sequence of bytes from the given [bytes](BufferController.Append(byte[],int,int).md#Be.Stateless.IO.BufferController.Append(byte[],int,int).bytes 'Be.Stateless.IO.BufferController.Append(byte[], int, int).bytes') array to the underlying controlled buffer. |
| [Append(byte[])](BufferController.Append(byte[]).md 'Be.Stateless.IO.BufferController.Append(byte[])') | Append an array of bytes to the underlying controlled buffer. |
| [Append(string, Encoding)](BufferController.Append(string,Encoding).md 'Be.Stateless.IO.BufferController.Append(string, System.Text.Encoding)') | Append the bytes making up a given string according to a specific encoding. |
| [Append(IEnumerable&lt;byte[]&gt;)](BufferController.Append(IEnumerable_byte[]_).md 'Be.Stateless.IO.BufferController.Append(System.Collections.Generic.IEnumerable<byte[]>)') | Append an [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of byte-array [buffers](BufferController.Append(IEnumerable_byte[]_).md#Be.Stateless.IO.BufferController.Append(System.Collections.Generic.IEnumerable_byte[]_).buffers 'Be.Stateless.IO.BufferController.Append(System.Collections.Generic.IEnumerable<byte[]>).buffers') to the underlying controlled buffer. |
| [Append(Func&lt;byte[],int,int,int&gt;)](BufferController.Append(Func_byte[],int,int,int_).md 'Be.Stateless.IO.BufferController.Append(System.Func<byte[],int,int,int>)') | Append to the underlying buffer by delegation. |
