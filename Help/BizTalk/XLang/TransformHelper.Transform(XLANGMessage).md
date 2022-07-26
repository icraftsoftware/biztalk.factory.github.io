#### [Be.Stateless.BizTalk.XLang](README.md 'README')
### [Be.Stateless.BizTalk.XLang](Be.Stateless.BizTalk.XLang.md 'Be.Stateless.BizTalk.XLang').[TransformHelper](TransformHelper.md 'Be.Stateless.BizTalk.XLang.TransformHelper')

## TransformHelper.Transform(XLANGMessage) Method

Applies the XSL transformation provided by the [message](TransformHelper.Transform(XLANGMessage).md#Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage).message 'Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage).message') context's [BizTalkFactoryProperties.MapTypeName](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.MapTypeName 'Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.MapTypeName') property to the specified
[message](TransformHelper.Transform(XLANGMessage).md#Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage).message 'Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage).message').

```csharp
public static Microsoft.XLANGs.BaseTypes.XLANGMessage Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage message);
```
#### Parameters

<a name='Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage).message'></a>

`message` [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')

The [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage') to be transformed.

#### Returns
[Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')  
The transformed message with the result in the first part (at index 0).

### Remarks

This method assumes only the first part of a multi-part [message](TransformHelper.Transform(XLANGMessage).md#Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage).message 'Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage).message') message has to be transformed and
creates an output message with a single part named "Main".

This method will throw if the map type to apply cannot be retrieved from the message context's [BizTalkFactoryProperties.MapTypeName](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.MapTypeName 'Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.MapTypeName') property.