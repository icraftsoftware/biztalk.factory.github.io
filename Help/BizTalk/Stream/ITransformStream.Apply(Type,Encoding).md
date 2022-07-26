#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream.Extensions](Be.Stateless.BizTalk.Stream.Extensions.md 'Be.Stateless.BizTalk.Stream.Extensions').[ITransformStream](ITransformStream.md 'Be.Stateless.BizTalk.Stream.Extensions.ITransformStream')

## ITransformStream.Apply(Type, Encoding) Method

Applies the [Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase')-derived transform on the current [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream'), or [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')s, and returns the results as another [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream').

```csharp
System.IO.Stream Apply(System.Type transform, System.Text.Encoding encoding);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Stream.Extensions.ITransformStream.Apply(System.Type,System.Text.Encoding).transform'></a>

`transform` [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')

The [Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase')-derived type of the transform to apply.

<a name='Be.Stateless.BizTalk.Stream.Extensions.ITransformStream.Apply(System.Type,System.Text.Encoding).encoding'></a>

`encoding` [System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding')

The encoding to use for the output [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream').

#### Returns
[System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')  
The output [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') being the results of the transform.