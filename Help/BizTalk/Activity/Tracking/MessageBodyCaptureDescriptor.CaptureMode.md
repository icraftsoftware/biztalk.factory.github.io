#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking](Be.Stateless.BizTalk.Activity.Tracking.md 'Be.Stateless.BizTalk.Activity.Tracking').[MessageBodyCaptureDescriptor](MessageBodyCaptureDescriptor.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureDescriptor')

## MessageBodyCaptureDescriptor.CaptureMode Property

Whether the payload of a message body is being captured directly into the BAM monitoring database or not, see
[Unclaimed](MessageBodyCaptureMode.md#Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Unclaimed 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Unclaimed') and [Claimed](MessageBodyCaptureMode.md#Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Claimed 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Claimed')
respectively.

```csharp
public Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode CaptureMode { get; }
```

#### Property Value
[MessageBodyCaptureMode](MessageBodyCaptureMode.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode')

### Remarks
If it equals to [Unclaimed](MessageBodyCaptureMode.md#Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Unclaimed 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Unclaimed'), [Data](MessageBodyCaptureDescriptor.Data.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureDescriptor.Data') denotes the actual payload of the
message body compressed and encoded as a Base64 string. If it is equals to [Claimed](MessageBodyCaptureMode.md#Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Claimed 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Claimed'), [Data](MessageBodyCaptureDescriptor.Data.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureDescriptor.Data') denotes the relative path to a file in the claim store
where the message body stream will be, or has been, committed to.