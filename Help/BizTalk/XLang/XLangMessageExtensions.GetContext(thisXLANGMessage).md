#### [Be.Stateless.BizTalk.XLang](README.md 'README')
### [Be.Stateless.BizTalk.XLang.Extensions](Be.Stateless.BizTalk.XLang.Extensions.md 'Be.Stateless.BizTalk.XLang.Extensions').[XLangMessageExtensions](XLangMessageExtensions.md 'Be.Stateless.BizTalk.XLang.Extensions.XLangMessageExtensions')

## XLangMessageExtensions.GetContext(this XLANGMessage) Method

Retrieves the context of an [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage') message.

```csharp
public static Microsoft.XLANGs.Core.XmlQNameTable GetContext(this Microsoft.XLANGs.BaseTypes.XLANGMessage message);
```
#### Parameters

<a name='Be.Stateless.BizTalk.XLang.Extensions.XLangMessageExtensions.GetContext(thisMicrosoft.XLANGs.BaseTypes.XLANGMessage).message'></a>

`message` [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')

The message whose context has to be retrieved.

#### Returns
[Microsoft.XLANGs.Core.XmlQNameTable](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.Core.XmlQNameTable 'Microsoft.XLANGs.Core.XmlQNameTable')  
The context of the [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')[message](XLangMessageExtensions.GetContext(thisXLANGMessage).md#Be.Stateless.BizTalk.XLang.Extensions.XLangMessageExtensions.GetContext(thisMicrosoft.XLANGs.BaseTypes.XLANGMessage).message 'Be.Stateless.BizTalk.XLang.Extensions.XLangMessageExtensions.GetContext(this Microsoft.XLANGs.BaseTypes.XLANGMessage).message').

### Remarks
Iterate over all segments in the current orchestration in search of the specified message object and return a
collection of context properties.

### See Also
- [Retrieving the Context of a BizTalk Message from an Orchestration](https://maximelabelle.wordpress.com/2011/01/07/retrieving-the-context-of-a-biztalk-message-from-an-orchestration/ 'https://maximelabelle.wordpress.com/2011/01/07/retrieving-the-context-of-a-biztalk-message-from-an-orchestration/')
- [Enumerating context properties](https://tsabar.wordpress.com/2009/12/02/enumerating-context-properties/ 'https://tsabar.wordpress.com/2009/12/02/enumerating-context-properties/')