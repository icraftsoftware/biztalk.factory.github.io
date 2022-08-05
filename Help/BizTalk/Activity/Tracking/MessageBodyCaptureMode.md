#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking](Be.Stateless.BizTalk.Activity.Tracking.md 'Be.Stateless.BizTalk.Activity.Tracking')

## MessageBodyCaptureMode Enum

Denotes whether a message's payload has been captured directly in the BAM monitoring database or not.

```csharp
public enum MessageBodyCaptureMode
```
### Fields

<a name='Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Claimed'></a>

`Claimed` 0

Denotes a message whose payload has been saved, or claimed, to disk and not directly captured in the BAM monitoring
database.

<a name='Be.Stateless.BizTalk.Activity.Tracking.MessageBodyCaptureMode.Unclaimed'></a>

`Unclaimed` 1

Denotes a message body whose payload has not been saved, or claimed, to disk but instead directly captured in the BAM
monitoring database.