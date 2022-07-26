#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream.Extensions](Be.Stateless.BizTalk.Stream.Extensions.md 'Be.Stateless.BizTalk.Stream.Extensions').[ITransformStream](ITransformStream.md 'Be.Stateless.BizTalk.Stream.Extensions.ITransformStream')

## ITransformStream.ExtendWith(IBaseMessageContext) Method

Provides extension objects that the [Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase')-derived transform might need.

```csharp
Be.Stateless.BizTalk.Stream.Extensions.ITransformStream ExtendWith(Microsoft.BizTalk.Message.Interop.IBaseMessageContext context);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Stream.Extensions.ITransformStream.ExtendWith(Microsoft.BizTalk.Message.Interop.IBaseMessageContext).context'></a>

`context` [Microsoft.BizTalk.Message.Interop.IBaseMessageContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessageContext 'Microsoft.BizTalk.Message.Interop.IBaseMessageContext')

The [Microsoft.BizTalk.Message.Interop.IBaseMessageContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessageContext 'Microsoft.BizTalk.Message.Interop.IBaseMessageContext') that will be later on passed as an extension object to the [Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase')-derived transform should it require it, see [Be.Stateless.BizTalk.Xml.Xsl.XslCompiledTransformDescriptor.ExtensionRequirements](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Xml.Xsl.XslCompiledTransformDescriptor.ExtensionRequirements 'Be.Stateless.BizTalk.Xml.Xsl.XslCompiledTransformDescriptor.ExtensionRequirements').

#### Returns
[ITransformStream](ITransformStream.md 'Be.Stateless.BizTalk.Stream.Extensions.ITransformStream')  
The [ITransformStream](ITransformStream.md 'Be.Stateless.BizTalk.Stream.Extensions.ITransformStream') instance that will apply the transform on the current [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream').