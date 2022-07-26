#### [Be.Stateless.BizTalk.XLang](README.md 'README')
### [Be.Stateless.BizTalk.XLang](Be.Stateless.BizTalk.XLang.md 'Be.Stateless.BizTalk.XLang').[SubOrchestrationFailedException](SubOrchestrationFailedException.md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException')

## SubOrchestrationFailedException.Throw(Exception) Method

XLang helper to throw a [SubOrchestrationFailedException](SubOrchestrationFailedException.md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException') with an [inner](SubOrchestrationFailedException.Throw(Exception).md#Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.Throw(System.Exception).inner 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.Throw(System.Exception).inner')[System.Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Exception 'System.Exception').

```csharp
public static void Throw(System.Exception inner);
```
#### Parameters

<a name='Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.Throw(System.Exception).inner'></a>

`inner` [System.Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Exception 'System.Exception')

The inner exception.

### Remarks
If the direct caller of this method is an orchestration, i.e. a [Microsoft.BizTalk.XLANGs.BTXEngine.BTXService](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.XLANGs.BTXEngine.BTXService 'Microsoft.BizTalk.XLANGs.BTXEngine.BTXService')-derived type, the thrown
[SubOrchestrationFailedException](SubOrchestrationFailedException.md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException')'s [Name](SubOrchestrationFailedException.Name.md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.Name') will be initialized to this orchestration's
namespace, which by convention is its name. If the direct caller is not an orchestration, then the [Name](SubOrchestrationFailedException.Name.md 'Be.Stateless.BizTalk.XLang.SubOrchestrationFailedException.Name')
will be initialized to the [Microsoft.XLANGs.Core.Service.RootService](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.Core.Service.RootService 'Microsoft.XLANGs.Core.Service.RootService')'s [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type') namespace.