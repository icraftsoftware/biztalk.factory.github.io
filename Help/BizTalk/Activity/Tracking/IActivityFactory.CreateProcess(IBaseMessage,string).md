#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Messaging](Be.Stateless.BizTalk.Activity.Tracking.Messaging.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging').[IActivityFactory](IActivityFactory.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.IActivityFactory')

## IActivityFactory.CreateProcess(IBaseMessage, string) Method

Creates a [Process](Process.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process') tracking activity denoting a process yet to be tracked.

```csharp
Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process CreateProcess(Microsoft.BizTalk.Message.Interop.IBaseMessage message, string name);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Messaging.IActivityFactory.CreateProcess(Microsoft.BizTalk.Message.Interop.IBaseMessage,string).message'></a>

`message` [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage')

The [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage') to which will be attached the ambient [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') referencing the
activity id of the current [Process](Process.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process').

<a name='Be.Stateless.BizTalk.Activity.Tracking.Messaging.IActivityFactory.CreateProcess(Microsoft.BizTalk.Message.Interop.IBaseMessage,string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name of the process to create.

#### Returns
[Process](Process.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process')  
A [Process](Process.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.Process') instance that will be used to feed the BAM Process activity.