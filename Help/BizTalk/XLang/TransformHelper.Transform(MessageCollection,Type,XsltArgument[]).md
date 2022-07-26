#### [Be.Stateless.BizTalk.XLang](README.md 'README')
### [Be.Stateless.BizTalk.XLang](Be.Stateless.BizTalk.XLang.md 'Be.Stateless.BizTalk.XLang').[TransformHelper](TransformHelper.md 'Be.Stateless.BizTalk.XLang.TransformHelper')

## TransformHelper.Transform(MessageCollection, Type, XsltArgument[]) Method

Applies the XSL transformation specified by [map](TransformHelper.Transform(MessageCollection,Type,XsltArgument[]).md#Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Be.Stateless.BizTalk.XLang.MessageCollection,System.Type,Be.Stateless.Xml.Xsl.XsltArgument[]).map 'Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Be.Stateless.BizTalk.XLang.MessageCollection, System.Type, Be.Stateless.Xml.Xsl.XsltArgument[]).map') to the specified [messages](TransformHelper.Transform(MessageCollection,Type,XsltArgument[]).md#Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Be.Stateless.BizTalk.XLang.MessageCollection,System.Type,Be.Stateless.Xml.Xsl.XsltArgument[]).messages 'Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Be.Stateless.BizTalk.XLang.MessageCollection, System.Type, Be.Stateless.Xml.Xsl.XsltArgument[]).messages').

```csharp
public static Microsoft.XLANGs.BaseTypes.XLANGMessage Transform(Be.Stateless.BizTalk.XLang.MessageCollection messages, System.Type map, params Be.Stateless.Xml.Xsl.XsltArgument[] arguments);
```
#### Parameters

<a name='Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Be.Stateless.BizTalk.XLang.MessageCollection,System.Type,Be.Stateless.Xml.Xsl.XsltArgument[]).messages'></a>

`messages` [MessageCollection](MessageCollection.md 'Be.Stateless.BizTalk.XLang.MessageCollection')

The [MessageCollection](MessageCollection.md 'Be.Stateless.BizTalk.XLang.MessageCollection') to be transformed.

<a name='Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Be.Stateless.BizTalk.XLang.MessageCollection,System.Type,Be.Stateless.Xml.Xsl.XsltArgument[]).map'></a>

`map` [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')

The type of the BizTalk map class containing the transform to apply.

<a name='Be.Stateless.BizTalk.XLang.TransformHelper.Transform(Be.Stateless.BizTalk.XLang.MessageCollection,System.Type,Be.Stateless.Xml.Xsl.XsltArgument[]).arguments'></a>

`arguments` [Be.Stateless.Xml.Xsl.XsltArgument](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.Xml.Xsl.XsltArgument 'Be.Stateless.Xml.Xsl.XsltArgument')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

The arguments to pass to the XSL transformation.

#### Returns
[Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')  
The transformed message with the result in the first part (at index 0).