#### [Be.Stateless.BizTalk.XLang](README.md 'README')
### [Be.Stateless.BizTalk.XLang](Be.Stateless.BizTalk.XLang.md 'Be.Stateless.BizTalk.XLang').[TransformHelper](TransformHelper.md 'Be.Stateless.BizTalk.XLang.TransformHelper')

## TransformHelper.Transform(XLANGMessage, XsltArgument[]) Method

Applies the XSL transformation provided by the [message](TransformHelper.Transform(XLANGMessage,XsltArgument[]).md#Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.Xml.Xsl.XsltArgument[]).message 'Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage, Be.Stateless.Xml.Xsl.XsltArgument[]).message') context's [BizTalkFactoryProperties.MapTypeName](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.MapTypeName 'Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.MapTypeName') property to the specified
[message](TransformHelper.Transform(XLANGMessage,XsltArgument[]).md#Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.Xml.Xsl.XsltArgument[]).message 'Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage, Be.Stateless.Xml.Xsl.XsltArgument[]).message').

```csharp
public static Microsoft.XLANGs.BaseTypes.XLANGMessage Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage message, params Be.Stateless.Xml.Xsl.XsltArgument[] arguments);
```
#### Parameters

<a name='Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.Xml.Xsl.XsltArgument[]).message'></a>

`message` [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')

The [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage') to be transformed.

<a name='Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.Xml.Xsl.XsltArgument[]).arguments'></a>

`arguments` [Be.Stateless.Xml.Xsl.XsltArgument](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.Xml.Xsl.XsltArgument 'Be.Stateless.Xml.Xsl.XsltArgument')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

The arguments to pass to the XSL transformation.

#### Returns
[Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')  
The transformed message with the result in the first part (at index 0).

### Remarks

This method assumes only the first part of a multi-part [message](TransformHelper.Transform(XLANGMessage,XsltArgument[]).md#Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage,Be.Stateless.Xml.Xsl.XsltArgument[]).message 'Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Microsoft.XLANGs.BaseTypes.XLANGMessage, Be.Stateless.Xml.Xsl.XsltArgument[]).message') message has to be transformed and
creates an output message with a single part named "Main".

This method will throw if the map type to apply cannot be retrieved from the message context's [BizTalkFactoryProperties.MapTypeName](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.MapTypeName 'Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.MapTypeName') property.