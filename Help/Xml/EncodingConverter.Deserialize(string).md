#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Text](Be.Stateless.Text.md 'Be.Stateless.Text').[EncodingConverter](EncodingConverter.md 'Be.Stateless.Text.EncodingConverter')

## EncodingConverter.Deserialize(string) Method

Converts the given [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') to a [System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding') instance.

```csharp
public static System.Text.Encoding Deserialize(string encoding);
```
#### Parameters

<a name='Be.Stateless.Text.EncodingConverter.Deserialize(string).encoding'></a>

`encoding` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') to convert to a [System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding') instance.

#### Returns
[System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding')  
A [System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding') instance that represents the converted [encoding](EncodingConverter.Deserialize(string).md#Be.Stateless.Text.EncodingConverter.Deserialize(string).encoding 'Be.Stateless.Text.EncodingConverter.Deserialize(string).encoding').

#### Exceptions

[System.NotSupportedException](https://docs.microsoft.com/en-us/dotnet/api/System.NotSupportedException 'System.NotSupportedException')  
The conversion cannot be performed.

### Remarks
An [System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding') can be converted back to a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') via the [Serialize(Encoding)](EncodingConverter.Serialize(Encoding).md 'Be.Stateless.Text.EncodingConverter.Serialize(System.Text.Encoding)')
methods.

### See Also
- [Serialize(Encoding)](EncodingConverter.Serialize(Encoding).md 'Be.Stateless.Text.EncodingConverter.Serialize(System.Text.Encoding)')