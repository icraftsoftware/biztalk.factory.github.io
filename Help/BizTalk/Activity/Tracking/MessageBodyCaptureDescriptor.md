#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking](Be.Stateless.BizTalk.Activity.Tracking.md 'Be.Stateless.BizTalk.Activity.Tracking')

## MessageBodyCaptureDescriptor Class

Describes how and where a message payload stream will be, or has been, captured.

```csharp
public class MessageBodyCaptureDescriptor
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; MessageBodyCaptureDescriptor

### Remarks

A [MessageBodyCaptureDescriptor](MessageBodyCaptureDescriptor.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureDescriptor') describes how a message body is being captured so that it could be both
tracked in the BAM monitoring database or participate in a claim-check MEP.

A [MessageBodyCaptureDescriptor](MessageBodyCaptureDescriptor.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureDescriptor') whose [CaptureMode](MessageBodyCaptureDescriptor.CaptureMode.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureDescriptor.CaptureMode') is equal to [Unclaimed](MessageBodyCaptureMode.md#Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Unclaimed 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Unclaimed') denotes a message body whose payload is being captured directly in the BAM
monitoring database. In this case, [Data](MessageBodyCaptureDescriptor.Data.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureDescriptor.Data') denotes the actual data that are going to be stored in the
monitoring database; specifically, the actual message body payload compressed and encoded as a Base64 string.

A [MessageBodyCaptureDescriptor](MessageBodyCaptureDescriptor.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureDescriptor') whose [CaptureMode](MessageBodyCaptureDescriptor.CaptureMode.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureDescriptor.CaptureMode') is equal to [Claimed](MessageBodyCaptureMode.md#Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Claimed 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Claimed') denotes a message body whose payload is being captured outside of the BAM
monitoring database. In this case, [Data](MessageBodyCaptureDescriptor.Data.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureDescriptor.Data') denotes the relative path to a file in the claim store where the
message body stream will be, or has been, committed to.

| Properties | |
| :--- | :--- |
| [CaptureMode](MessageBodyCaptureDescriptor.CaptureMode.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureDescriptor.CaptureMode') | Whether the payload of a message body is being captured directly into the BAM monitoring database or not, see [Unclaimed](MessageBodyCaptureMode.md#Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Unclaimed 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Unclaimed') and [Claimed](MessageBodyCaptureMode.md#Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Claimed 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Claimed') respectively. |
| [Data](MessageBodyCaptureDescriptor.Data.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureDescriptor.Data') | Either the message body's actual payload or the relative path to a file in the claim store where the message body stream will be, or has been, committed to. |
