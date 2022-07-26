#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO').[BufferController](BufferController.md 'Be.Stateless.IO.BufferController')

## BufferController.Append(string, Encoding) Method

Append the bytes making up a given string according to a specific encoding.

```csharp
public byte[] Append(string @string, System.Text.Encoding encoding);
```
#### Parameters

<a name='Be.Stateless.IO.BufferController.Append(string,System.Text.Encoding).string'></a>

`string` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The string whose bytes will be appended to the buffer.

<a name='Be.Stateless.IO.BufferController.Append(string,System.Text.Encoding).encoding'></a>

`encoding` [System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding')

The encoding according to which the string must be converted to bytes.

#### Returns
[System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')  
The array of bytes that could not be appended to the underlying controlled buffer because of availability shortage.