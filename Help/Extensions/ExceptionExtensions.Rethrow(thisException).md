#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Extensions](Be.Stateless.Extensions.md 'Be.Stateless.Extensions').[ExceptionExtensions](ExceptionExtensions.md 'Be.Stateless.Extensions.ExceptionExtensions')

## ExceptionExtensions.Rethrow(this Exception) Method

Rethrows an [exception](ExceptionExtensions.Rethrow(thisException).md#Be.Stateless.Extensions.ExceptionExtensions.Rethrow(thisSystem.Exception).exception 'Be.Stateless.Extensions.ExceptionExtensions.Rethrow(this System.Exception).exception'), maintaining the original Watson information and augmenting rather than
replacing the original stack trace.

```csharp
public static void Rethrow(this System.Exception exception);
```
#### Parameters

<a name='Be.Stateless.Extensions.ExceptionExtensions.Rethrow(thisSystem.Exception).exception'></a>

`exception` [System.Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Exception 'System.Exception')

The exception to be rethrown.

### See Also
- [ExceptionDispatchInfo.Capture](https://docs.microsoft.com/en-us/dotnet/api/System.Runtime.ExceptionServices.ExceptionDispatchInfo.Capture#System_Runtime_ExceptionServices_ExceptionDispatchInfo_Capture_System_Exception_ 'System.Runtime.ExceptionServices.ExceptionDispatchInfo.Capture(System.Exception)')
- [ExceptionDispatchInfo.Throw](https://docs.microsoft.com/en-us/dotnet/api/System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw 'System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw')
- [How to rethrow InnerException without losing stack trace in C#?](https://stackoverflow.com/a/17091351/1789441 'https://stackoverflow.com/a/17091351/1789441')