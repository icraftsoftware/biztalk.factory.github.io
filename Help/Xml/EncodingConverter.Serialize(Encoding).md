#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Text](Be.Stateless.Text.md 'Be.Stateless.Text').[EncodingConverter](EncodingConverter.md 'Be.Stateless.Text.EncodingConverter')

## EncodingConverter.Serialize(Encoding) Method

Converts a [System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding') instance to its [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') representation.

```csharp
public static string Serialize(System.Text.Encoding encoding);
```
#### Parameters

<a name='Be.Stateless.Text.EncodingConverter.Serialize(System.Text.Encoding).encoding'></a>

`encoding` [System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding')

The [System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding') instance to serialize.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
A [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') that represents the [System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding').

### Remarks

The serialization format of an encoding is as follows `<Name>[ with signature]` where
`<Name>` is the [System.Text.Encoding.WebName](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding.WebName 'System.Text.Encoding.WebName') of the encoding and `with signature` is an
optional modifier that is present only for a Unicode encoding if a byte order mark preamble has be emitted.

The [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') serialized representation of an [System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding') can be converted back to an
[System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding') via the [Deserialize(string)](EncodingConverter.Deserialize(string).md 'Be.Stateless.Text.EncodingConverter.Deserialize(string)') methods.

### See Also
- [Deserialize(string)](EncodingConverter.Deserialize(string).md 'Be.Stateless.Text.EncodingConverter.Deserialize(string)')