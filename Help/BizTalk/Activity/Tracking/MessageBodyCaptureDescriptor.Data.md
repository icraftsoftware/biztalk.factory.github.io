#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking](Be.Stateless.BizTalk.Activity.Tracking.md 'Be.Stateless.BizTalk.Activity.Tracking').[MessageBodyCaptureDescriptor](MessageBodyCaptureDescriptor.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureDescriptor')

## MessageBodyCaptureDescriptor.Data Property

Either the message body's actual payload or the relative path to a file in the claim store where the message body
stream will be, or has been, committed to.

```csharp
public string Data { get; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
If [CaptureMode](MessageBodyCaptureDescriptor.CaptureMode.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureDescriptor.CaptureMode') is equals to [Unclaimed](MessageBodyCaptureMode.md#Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Unclaimed 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Unclaimed'), it denotes the actual
payload of the message body compressed and encoded as a Base64 string. If [CaptureMode](MessageBodyCaptureDescriptor.CaptureMode.md 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureDescriptor.CaptureMode') is equals to [Claimed](MessageBodyCaptureMode.md#Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Claimed 'Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Claimed'), it denotes the relative path to a file in the claim store where the message
body stream will be, or has been, committed to.