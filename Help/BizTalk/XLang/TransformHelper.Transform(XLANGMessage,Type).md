#### [Be.Stateless.BizTalk.XLang](README.md 'README')
### [Be.Stateless.BizTalk.XLang](Be.Stateless.BizTalk.XLang.md 'Be.Stateless.BizTalk.XLang').[TransformHelper](TransformHelper.md 'Be.Stateless.BizTalk.XLang.TransformHelper')

## TransformHelper.Transform(XLANGMessage, Type) Method

Applies the XSL transformation specified by [map](TransformHelper.Transform(XLANGMessage,Type).md#Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage,System.Type).map 'Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage, System.Type).map') to the specified [message](TransformHelper.Transform(XLANGMessage,Type).md#Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage,System.Type).message 'Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage, System.Type).message').

```csharp
public static Microsoft.XLANGs.BaseTypes.XLANGMessage Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage message, System.Type map);
```
#### Parameters

<a name='Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage,System.Type).message'></a>

`message` [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')

The [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage') to be transformed.

<a name='Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage,System.Type).map'></a>

`map` [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')

The type of the BizTalk map class containing the transform to apply.

#### Returns
[Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')  
The transformed message with the result in the first part (at index 0).

### Remarks
This method assumes only the first part of a multi-part [message](TransformHelper.Transform(XLANGMessage,Type).md#Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage,System.Type).message 'Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage, System.Type).message') message has to be transformed and
creates an output message with a single part named "Main".