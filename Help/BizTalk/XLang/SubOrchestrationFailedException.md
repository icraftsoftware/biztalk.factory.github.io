#### [Be.Stateless.BizTalk.XLang](README.md 'README')
### [Be.Stateless.BizTalk.XLang](Be.Stateless.BizTalk.XLang.md 'Be.Stateless.BizTalk.XLang')

## SubOrchestrationFailedException Class

In the context of BizTalk Server composite orchestrations, allows a sub-orchestration to notify its caller that it has
failed by throwing a [SubOrchestrationFailedException](SubOrchestrationFailedException.md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException') that identifies it by its [Name](SubOrchestrationFailedException.Name.md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.Name').

```csharp
public class SubOrchestrationFailedException : System.Exception
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Exception 'System.Exception') &#129106; SubOrchestrationFailedException

Derived  
&#8627; [SubOrchestrationFailedException](SubOrchestrationFailedException.md 'BizTalk.Factory.XLang.SubOrchestrationFailedException')

| Constructors | |
| :--- | :--- |
| [SubOrchestrationFailedException(string, string, Exception)](SubOrchestrationFailedException.SubOrchestrationFailedException(string,string,Exception).md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.SubOrchestrationFailedException(string, string, System.Exception)') | |
| [SubOrchestrationFailedException(string, string)](SubOrchestrationFailedException.SubOrchestrationFailedException(string,string).md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.SubOrchestrationFailedException(string, string)') | |
| [SubOrchestrationFailedException(SerializationInfo, StreamingContext)](SubOrchestrationFailedException.SubOrchestrationFailedException(SerializationInfo,StreamingContext).md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.SubOrchestrationFailedException(System.Runtime.Serialization.SerializationInfo, System.Runtime.Serialization.StreamingContext)') | |

| Properties | |
| :--- | :--- |
| [Message](SubOrchestrationFailedException.Message.md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.Message') | |
| [Name](SubOrchestrationFailedException.Name.md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.Name') | The name of the sub-orchestration that has failed and thrown this exception. |

| Methods | |
| :--- | :--- |
| [GetObjectData(SerializationInfo, StreamingContext)](SubOrchestrationFailedException.GetObjectData(SerializationInfo,StreamingContext).md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.GetObjectData(System.Runtime.Serialization.SerializationInfo, System.Runtime.Serialization.StreamingContext)') | |
| [Throw()](SubOrchestrationFailedException.Throw().md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.Throw()') | XLang helper to throw a [SubOrchestrationFailedException](SubOrchestrationFailedException.md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException'). |
| [Throw(Exception)](SubOrchestrationFailedException.Throw(Exception).md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.Throw(System.Exception)') | XLang helper to throw a [SubOrchestrationFailedException](SubOrchestrationFailedException.md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException') with an [inner](SubOrchestrationFailedException.Throw(Exception).md#Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.Throw(System.Exception).inner 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.Throw(System.Exception).inner')[System.Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Exception 'System.Exception'). |
