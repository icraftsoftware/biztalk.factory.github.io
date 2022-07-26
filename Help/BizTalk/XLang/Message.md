#### [Be.Stateless.BizTalk.XLang](README.md 'README')
### [Be.Stateless.BizTalk.XLang](Be.Stateless.BizTalk.XLang.md 'Be.Stateless.BizTalk.XLang')

## Message Class

```csharp
public sealed class Message : Microsoft.BizTalk.XLANGs.BTXEngine.BTXMessage
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage') &#129106; [Microsoft.XLANGs.Core.XMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.Core.XMessage 'Microsoft.XLANGs.Core.XMessage') &#129106; [Microsoft.BizTalk.XLANGs.BTXEngine.BTXMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.XLANGs.BTXEngine.BTXMessage 'Microsoft.BizTalk.XLANGs.BTXEngine.BTXMessage') &#129106; Message

| Methods | |
| :--- | :--- |
| [Create(Context, Stream)](Message.Create(Context,Stream).md 'Be.Stateless.BizTalk.XLang.Message.Create(Microsoft.XLANGs.Core.Context, System.IO.Stream)') | |
| [Create(Context, XmlDocument)](Message.Create(Context,XmlDocument).md 'Be.Stateless.BizTalk.XLang.Message.Create(Microsoft.XLANGs.Core.Context, System.Xml.XmlDocument)') | |
| [PromoteMessageType(XLANGMessage)](Message.PromoteMessageType(XLANGMessage).md 'Be.Stateless.BizTalk.XLang.Message.PromoteMessageType(Microsoft.XLANGs.BaseTypes.XLANGMessage)') | Promotes the [BTS.MessageType](https://docs.microsoft.com/en-us/dotnet/api/BTS.MessageType 'BTS.MessageType') of an untyped —typically [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')— [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')[message](Message.PromoteMessageType(XLANGMessage).md#Be.Stateless.BizTalk.XLang.Message.PromoteMessageType(Microsoft.XLANGs.BaseTypes.XLANGMessage).message 'Be.Stateless.BizTalk.XLang.Message.PromoteMessageType(Microsoft.XLANGs.BaseTypes.XLANGMessage).message') from within an orchestration. |
