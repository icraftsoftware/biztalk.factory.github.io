#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking](Be.Stateless.BizTalk.Activity.Tracking.md 'Be.Stateless.BizTalk.Activity.Tracking')

## ActivityTrackingModes Enum

Policy denoting to what extent a messaging activity will be tracked.

```csharp
public enum ActivityTrackingModes
```
### Fields

<a name='Be.Stateless.BizTalk.Activity.Tracking.ActivityTrackingModes.Body'></a>

`Body` 7

Track the messaging step together with its context and payload data.

<a name='Be.Stateless.BizTalk.Activity.Tracking.ActivityTrackingModes.Claim'></a>

`Claim` 15

Track the messaging step together with its context and payload data. Moreover the payload data will be claimed to
disk and replaced by a `Claim.Check` token.

<a name='Be.Stateless.BizTalk.Activity.Tracking.ActivityTrackingModes.Context'></a>

`Context` 3

Track the messaging step together with its context data, but without payload data.

<a name='Be.Stateless.BizTalk.Activity.Tracking.ActivityTrackingModes.None'></a>

`None` 0

Do not track the messaging step at all.

<a name='Be.Stateless.BizTalk.Activity.Tracking.ActivityTrackingModes.Step'></a>

`Step` 1

Track the messaging step without any context or payload data.