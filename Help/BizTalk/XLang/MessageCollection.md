#### [Be.Stateless.BizTalk.XLang](README.md 'README')
### [Be.Stateless.BizTalk.XLang](Be.Stateless.BizTalk.XLang.md 'Be.Stateless.BizTalk.XLang')

## MessageCollection Class

A collection of [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage') messages that facilitates calling of [TransformHelper](TransformHelper.md 'Be.Stateless.BizTalk.XLang.TransformHelper') with
several messages from within an orchestration XLang expression shape.

```csharp
public class MessageCollection : System.Collections.Generic.LinkedList<Microsoft.XLANGs.BaseTypes.XLANGMessage>,
System.IDisposable
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.Collections.Generic.LinkedList&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.LinkedList-1 'System.Collections.Generic.LinkedList`1')[Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.LinkedList-1 'System.Collections.Generic.LinkedList`1') &#129106; MessageCollection

Derived  
&#8627; [MessageCollection](MessageCollection.md 'BizTalk.Factory.XLang.MessageCollection')

Implements [System.IDisposable](https://docs.microsoft.com/en-us/dotnet/api/System.IDisposable 'System.IDisposable')

| Constructors | |
| :--- | :--- |
| [MessageCollection()](MessageCollection.MessageCollection().md 'Be.Stateless.BizTalk.XLang.MessageCollection.MessageCollection()') | |
| [MessageCollection(XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage)](MessageCollection.MessageCollection(XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage).md 'Be.Stateless.BizTalk.XLang.MessageCollection.MessageCollection(Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage)') | |
| [MessageCollection(XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage)](MessageCollection.MessageCollection(XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage).md 'Be.Stateless.BizTalk.XLang.MessageCollection.MessageCollection(Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage)') | |
| [MessageCollection(XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage)](MessageCollection.MessageCollection(XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage).md 'Be.Stateless.BizTalk.XLang.MessageCollection.MessageCollection(Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage)') | |
| [MessageCollection(XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage)](MessageCollection.MessageCollection(XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage).md 'Be.Stateless.BizTalk.XLang.MessageCollection.MessageCollection(Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage)') | |
| [MessageCollection(XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage)](MessageCollection.MessageCollection(XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage).md 'Be.Stateless.BizTalk.XLang.MessageCollection.MessageCollection(Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage)') | |
| [MessageCollection(XLANGMessage, XLANGMessage, XLANGMessage, XLANGMessage)](MessageCollection.MessageCollection(XLANGMessage,XLANGMessage,XLANGMessage,XLANGMessage).md 'Be.Stateless.BizTalk.XLang.MessageCollection.MessageCollection(Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage)') | |
| [MessageCollection(XLANGMessage, XLANGMessage, XLANGMessage)](MessageCollection.MessageCollection(XLANGMessage,XLANGMessage,XLANGMessage).md 'Be.Stateless.BizTalk.XLang.MessageCollection.MessageCollection(Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage)') | |
| [MessageCollection(XLANGMessage, XLANGMessage)](MessageCollection.MessageCollection(XLANGMessage,XLANGMessage).md 'Be.Stateless.BizTalk.XLang.MessageCollection.MessageCollection(Microsoft.XLANGs.BaseTypes.XLANGMessage, Microsoft.XLANGs.BaseTypes.XLANGMessage)') | |
| [MessageCollection(XLANGMessage)](MessageCollection.MessageCollection(XLANGMessage).md 'Be.Stateless.BizTalk.XLang.MessageCollection.MessageCollection(Microsoft.XLANGs.BaseTypes.XLANGMessage)') | |

| Methods | |
| :--- | :--- |
| [Add(XLANGMessage)](MessageCollection.Add(XLANGMessage).md 'Be.Stateless.BizTalk.XLang.MessageCollection.Add(Microsoft.XLANGs.BaseTypes.XLANGMessage)') | |

| Operators | |
| :--- | :--- |
| [implicit operator XmlReader(MessageCollection)](MessageCollection.implicitoperatorXmlReader(MessageCollection).md 'Be.Stateless.BizTalk.XLang.MessageCollection.op_Implicit System.Xml.XmlReader(Be.Stateless.BizTalk.XLang.MessageCollection)') | |

| Explicit Interface Implementations | |
| :--- | :--- |
| [System.IDisposable.Dispose()](MessageCollection.System.IDisposable.Dispose().md 'Be.Stateless.BizTalk.XLang.MessageCollection.System.IDisposable.Dispose()') | |
