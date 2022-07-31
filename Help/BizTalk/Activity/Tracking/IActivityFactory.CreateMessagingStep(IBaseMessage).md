#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Messaging](Be.Stateless.BizTalk.Activity.Tracking.Messaging.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging').[IActivityFactory](IActivityFactory.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.IActivityFactory')

## IActivityFactory.CreateMessagingStep(IBaseMessage) Method

Creates a [MessagingStep](MessagingStep.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep') tracking activity denoting a message yet to be tracked.

```csharp
Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep CreateMessagingStep(Microsoft.BizTalk.Message.Interop.IBaseMessage message);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Messaging.IActivityFactory.CreateMessagingStep(Microsoft.BizTalk.Message.Interop.IBaseMessage).message'></a>

`message` [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage')

The [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage') whose [Microsoft.BizTalk.Message.Interop.IBaseMessage.BodyPart](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage.BodyPart 'Microsoft.BizTalk.Message.Interop.IBaseMessage.BodyPart') and [Microsoft.BizTalk.Message.Interop.IBaseMessageContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessageContext 'Microsoft.BizTalk.Message.Interop.IBaseMessageContext') data
will be fed to the BAM MessagingStep activity.

#### Returns
[MessagingStep](MessagingStep.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep')  
A [MessagingStep](MessagingStep.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.MessagingStep') instance that will be used to feed the BAM MessagingStep activity.