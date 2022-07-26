#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Extensions](Be.Stateless.Extensions.md 'Be.Stateless.Extensions').[ExceptionExtensions](ExceptionExtensions.md 'Be.Stateless.Extensions.ExceptionExtensions')

## ExceptionExtensions.IsFatal(this Exception) Method

Determines whether an exception is fatal, that is to say <b>unrecoverable</b>, or not.

```csharp
public static bool IsFatal(this System.Exception exception);
```
#### Parameters

<a name='Be.Stateless.Extensions.ExceptionExtensions.IsFatal(thisSystem.Exception).exception'></a>

`exception` [System.Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Exception 'System.Exception')

The exception to assess.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if [exception](ExceptionExtensions.IsFatal(thisException).md#Be.Stateless.Extensions.ExceptionExtensions.IsFatal(thisSystem.Exception).exception 'Be.Stateless.Extensions.ExceptionExtensions.IsFatal(this System.Exception).exception') is fatal; `false` otherwise.

### See Also
- [https://vasters.com/archive/Are-You-Catching-Falling-Knives.html](https://vasters.com/archive/Are-You-Catching-Falling-Knives.html 'https://vasters.com/archive/Are-You-Catching-Falling-Knives.html')