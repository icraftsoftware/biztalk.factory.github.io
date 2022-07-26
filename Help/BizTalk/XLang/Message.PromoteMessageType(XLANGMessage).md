#### [Be.Stateless.BizTalk.XLang](README.md 'README')
### [Be.Stateless.BizTalk.XLang](Be.Stateless.BizTalk.XLang.md 'Be.Stateless.BizTalk.XLang').[Message](Message.md 'Be.Stateless.BizTalk.XLang.Message')

## Message.PromoteMessageType(XLANGMessage) Method

Promotes the [BTS.MessageType](https://docs.microsoft.com/en-us/dotnet/api/BTS.MessageType 'BTS.MessageType') of an untyped —typically [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument')— [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')[message](Message.PromoteMessageType(XLANGMessage).md#Be.Stateless.BizTalk.XLang.Message.PromoteMessageType(Microsoft.XLANGs.BaseTypes.XLANGMessage).message 'Be.Stateless.BizTalk.XLang.Message.PromoteMessageType(Microsoft.XLANGs.BaseTypes.XLANGMessage).message') from within an orchestration.

```csharp
public static void PromoteMessageType(Microsoft.XLANGs.BaseTypes.XLANGMessage message);
```
#### Parameters

<a name='Be.Stateless.BizTalk.XLang.Message.PromoteMessageType(Microsoft.XLANGs.BaseTypes.XLANGMessage).message'></a>

`message` [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')

The untyped [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage') message whose [BTS.MessageType](https://docs.microsoft.com/en-us/dotnet/api/BTS.MessageType 'BTS.MessageType') needs to be promoted.

### Remarks

Messages sent to the message box using a direct send port are generally subscribed to by their destination
orchestrations or ports using a filter based on their message type. An untyped [message](Message.PromoteMessageType(XLANGMessage).md#Be.Stateless.BizTalk.XLang.Message.PromoteMessageType(Microsoft.XLANGs.BaseTypes.XLANGMessage).message 'Be.Stateless.BizTalk.XLang.Message.PromoteMessageType(Microsoft.XLANGs.BaseTypes.XLANGMessage).message') sent to the
message box through a direct send port, however, has by default no promoted properties, hence no [BTS.MessageType](https://docs.microsoft.com/en-us/dotnet/api/BTS.MessageType 'BTS.MessageType'), and will generally end up with a <i>routing failure</i> error.

The only property really needing to be promoted in this case is the [BTS.MessageType](https://docs.microsoft.com/en-us/dotnet/api/BTS.MessageType 'BTS.MessageType'); but within an
orchestration [BTS.MessageType](https://docs.microsoft.com/en-us/dotnet/api/BTS.MessageType 'BTS.MessageType') is <b>readonly</b>. To work around this issue entails invoking the [Microsoft.BizTalk.DefaultPipelines.XMLReceive](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.DefaultPipelines.XMLReceive 'Microsoft.BizTalk.DefaultPipelines.XMLReceive') pipeline within the orchestration, as it promotes a series of properties including in particular
the [BTS.MessageType](https://docs.microsoft.com/en-us/dotnet/api/BTS.MessageType 'BTS.MessageType').

Invoking a pipeline within an orchestration however requires an atomic scope, which is not necessary in our case and
be avoided by calling this helper method from within a message assignment or construction shape.

There is one last "<i>gotcha</i>". [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlDocument 'System.Xml.XmlDocument') messages sent to message box using a direct send port
will still drop their context and consequently their promoted [BTS.MessageType](https://docs.microsoft.com/en-us/dotnet/api/BTS.MessageType 'BTS.MessageType') property. A correlation
set including this very same [BTS.MessageType](https://docs.microsoft.com/en-us/dotnet/api/BTS.MessageType 'BTS.MessageType') property therefore still need to be defined and
initialized from within the orchestration.

### See Also
- [Promoting MessageType property on untyped messages](http://ronaldlokers.blogspot.com/2012/04/promoting-messagetype-property-on.html 'http://ronaldlokers.blogspot.com/2012/04/promoting-messagetype-property-on.html')