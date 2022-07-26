#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream.Extensions](Be.Stateless.BizTalk.Stream.Extensions.md 'Be.Stateless.BizTalk.Stream.Extensions').[StreamExtensions](StreamExtensions.md 'Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions')

## StreamExtensions.Transform(this Stream) Method

Support for [Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase')-derived transforms directly applied to one [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream').

```csharp
public static Be.Stateless.BizTalk.Stream.Extensions.ITransformStream Transform(this System.IO.Stream stream);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions.Transform(thisSystem.IO.Stream).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The current [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream').

#### Returns
[ITransformStream](ITransformStream.md 'Be.Stateless.BizTalk.Stream.Extensions.ITransformStream')  
The [ITransformStream](ITransformStream.md 'Be.Stateless.BizTalk.Stream.Extensions.ITransformStream') instance that will apply the transform on the current [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream').