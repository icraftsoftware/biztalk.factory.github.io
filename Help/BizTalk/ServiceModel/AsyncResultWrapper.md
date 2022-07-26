#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk](Be.Stateless.BizTalk.md 'Be.Stateless.BizTalk')

## AsyncResultWrapper Class

[System.IAsyncResult](https://docs.microsoft.com/en-us/dotnet/api/System.IAsyncResult 'System.IAsyncResult') wrapper to be used to wrap around another [System.IAsyncResult](https://docs.microsoft.com/en-us/dotnet/api/System.IAsyncResult 'System.IAsyncResult') when one wants to
            intercept an asynchronous call and provides his own user-defined [AsyncState](AsyncResultWrapper.AsyncState.md 'Be.Stateless.BizTalk.AsyncResultWrapper.AsyncState') object.

```csharp
public class AsyncResultWrapper :
System.IAsyncResult
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; AsyncResultWrapper

Implements [System.IAsyncResult](https://docs.microsoft.com/en-us/dotnet/api/System.IAsyncResult 'System.IAsyncResult')

### Remarks
See [BeginRelayRequest&lt;TRequest&gt;(TRequest, AsyncCallback, object)](ServiceRelay.BeginRelayRequest_TRequest_(TRequest,AsyncCallback,object).md 'Be.Stateless.BizTalk.ServiceModel.ServiceRelay.BeginRelayRequest<TRequest>(TRequest, System.AsyncCallback, object)') for sample usages.

### See Also
- [System.IAsyncResult](https://docs.microsoft.com/en-us/dotnet/api/System.IAsyncResult 'System.IAsyncResult')

| Constructors | |
| :--- | :--- |
| [AsyncResultWrapper(IAsyncResult, object)](AsyncResultWrapper.AsyncResultWrapper(IAsyncResult,object).md 'Be.Stateless.BizTalk.AsyncResultWrapper.AsyncResultWrapper(System.IAsyncResult, object)') | Initializes a new instance of the [AsyncResultWrapper](AsyncResultWrapper.md 'Be.Stateless.BizTalk.AsyncResultWrapper') around another specified [asyncResult](AsyncResultWrapper.AsyncResultWrapper(IAsyncResult,object).md#Be.Stateless.BizTalk.AsyncResultWrapper.AsyncResultWrapper(System.IAsyncResult,object).asyncResult 'Be.Stateless.BizTalk.AsyncResultWrapper.AsyncResultWrapper(System.IAsyncResult, object).asyncResult') and using the specified [asyncState](AsyncResultWrapper.AsyncResultWrapper(IAsyncResult,object).md#Be.Stateless.BizTalk.AsyncResultWrapper.AsyncResultWrapper(System.IAsyncResult,object).asyncState 'Be.Stateless.BizTalk.AsyncResultWrapper.AsyncResultWrapper(System.IAsyncResult, object).asyncState'). |

| Properties | |
| :--- | :--- |
| [AsyncState](AsyncResultWrapper.AsyncState.md 'Be.Stateless.BizTalk.AsyncResultWrapper.AsyncState') | Gets a user-defined [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') that qualifies or contains information about an asynchronous operation. |
| [AsyncWaitHandle](AsyncResultWrapper.AsyncWaitHandle.md 'Be.Stateless.BizTalk.AsyncResultWrapper.AsyncWaitHandle') | Gets a [System.Threading.WaitHandle](https://docs.microsoft.com/en-us/dotnet/api/System.Threading.WaitHandle 'System.Threading.WaitHandle') that is used to wait for an asynchronous operation to complete. |
| [CompletedSynchronously](AsyncResultWrapper.CompletedSynchronously.md 'Be.Stateless.BizTalk.AsyncResultWrapper.CompletedSynchronously') | Gets a value that indicates whether the asynchronous operation completed synchronously. |
| [IsCompleted](AsyncResultWrapper.IsCompleted.md 'Be.Stateless.BizTalk.AsyncResultWrapper.IsCompleted') | Gets a value that indicates whether the asynchronous operation has completed. |
| [WrappedAsyncResult](AsyncResultWrapper.WrappedAsyncResult.md 'Be.Stateless.BizTalk.AsyncResultWrapper.WrappedAsyncResult') | The wrapped [System.IAsyncResult](https://docs.microsoft.com/en-us/dotnet/api/System.IAsyncResult 'System.IAsyncResult'). |
