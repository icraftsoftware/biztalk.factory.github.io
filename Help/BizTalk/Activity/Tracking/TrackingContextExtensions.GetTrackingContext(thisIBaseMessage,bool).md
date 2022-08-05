#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Extensions](Be.Stateless.BizTalk.Activity.Tracking.Extensions.md 'Be.Stateless.BizTalk.Activity.Tracking.Extensions').[TrackingContextExtensions](TrackingContextExtensions.md 'Be.Stateless.BizTalk.Activity.Tracking.Extensions.TrackingContextExtensions')

## TrackingContextExtensions.GetTrackingContext(this IBaseMessage, bool) Method

Returns the [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') associated to the [message](TrackingContextExtensions.GetTrackingContext(thisIBaseMessage,bool).md#Be.Stateless.BizTalk.Activity.Tracking.Extensions.TrackingContextExtensions.GetTrackingContext(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,bool).message 'Be.Stateless.BizTalk.Activity.Tracking.Extensions.TrackingContextExtensions.GetTrackingContext(this Microsoft.BizTalk.Message.Interop.IBaseMessage, bool).message').

```csharp
public static Be.Stateless.BizTalk.Activity.Tracking.TrackingContext GetTrackingContext(this Microsoft.BizTalk.Message.Interop.IBaseMessage message, bool throwOnEmpty);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Extensions.TrackingContextExtensions.GetTrackingContext(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,bool).message'></a>

`message` [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage')

Message whose associated [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') will be returned.

<a name='Be.Stateless.BizTalk.Activity.Tracking.Extensions.TrackingContextExtensions.GetTrackingContext(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,bool).throwOnEmpty'></a>

`throwOnEmpty` [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

`true` to throw an [System.InvalidOperationException](https://docs.microsoft.com/en-us/dotnet/api/System.InvalidOperationException 'System.InvalidOperationException') if none of the discrete activity Ids of the [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') are set in the [message](TrackingContextExtensions.GetTrackingContext(thisIBaseMessage,bool).md#Be.Stateless.BizTalk.Activity.Tracking.Extensions.TrackingContextExtensions.GetTrackingContext(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,bool).message 'Be.Stateless.BizTalk.Activity.Tracking.Extensions.TrackingContextExtensions.GetTrackingContext(this Microsoft.BizTalk.Message.Interop.IBaseMessage, bool).message')'s context.

#### Returns
[TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext')  
The [TrackingContext](TrackingContext.md 'Be.Stateless.BizTalk.Activity.Tracking.TrackingContext') associated to the [message](TrackingContextExtensions.GetTrackingContext(thisIBaseMessage,bool).md#Be.Stateless.BizTalk.Activity.Tracking.Extensions.TrackingContextExtensions.GetTrackingContext(thisMicrosoft.BizTalk.Message.Interop.IBaseMessage,bool).message 'Be.Stateless.BizTalk.Activity.Tracking.Extensions.TrackingContextExtensions.GetTrackingContext(this Microsoft.BizTalk.Message.Interop.IBaseMessage, bool).message').