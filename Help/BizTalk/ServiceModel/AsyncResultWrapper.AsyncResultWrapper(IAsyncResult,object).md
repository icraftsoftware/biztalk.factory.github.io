#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk](Be.Stateless.BizTalk.md 'Be.Stateless.BizTalk').[AsyncResultWrapper](AsyncResultWrapper.md 'Be.Stateless.BizTalk.AsyncResultWrapper')

## AsyncResultWrapper(IAsyncResult, object) Constructor

Initializes a new instance of the [AsyncResultWrapper](AsyncResultWrapper.md 'Be.Stateless.BizTalk.AsyncResultWrapper') around another specified [asyncResult](AsyncResultWrapper.AsyncResultWrapper(IAsyncResult,object).md#Be.Stateless.BizTalk.AsyncResultWrapper.AsyncResultWrapper(System.IAsyncResult,object).asyncResult 'Be.Stateless.BizTalk.AsyncResultWrapper.AsyncResultWrapper(System.IAsyncResult, object).asyncResult') and using the specified [asyncState](AsyncResultWrapper.AsyncResultWrapper(IAsyncResult,object).md#Be.Stateless.BizTalk.AsyncResultWrapper.AsyncResultWrapper(System.IAsyncResult,object).asyncState 'Be.Stateless.BizTalk.AsyncResultWrapper.AsyncResultWrapper(System.IAsyncResult, object).asyncState').

```csharp
public AsyncResultWrapper(System.IAsyncResult asyncResult, object asyncState);
```
#### Parameters

<a name='Be.Stateless.BizTalk.AsyncResultWrapper.AsyncResultWrapper(System.IAsyncResult,object).asyncResult'></a>

`asyncResult` [System.IAsyncResult](https://docs.microsoft.com/en-us/dotnet/api/System.IAsyncResult 'System.IAsyncResult')

The [System.IAsyncResult](https://docs.microsoft.com/en-us/dotnet/api/System.IAsyncResult 'System.IAsyncResult') to wrap.

<a name='Be.Stateless.BizTalk.AsyncResultWrapper.AsyncResultWrapper(System.IAsyncResult,object).asyncState'></a>

`asyncState` [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')

A user-defined [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') that qualifies or contains information about an asynchronous operation.