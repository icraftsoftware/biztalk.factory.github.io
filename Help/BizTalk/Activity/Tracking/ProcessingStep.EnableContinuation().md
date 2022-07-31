#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Messaging](Be.Stateless.BizTalk.Activity.Tracking.Messaging.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging').[ProcessingStep](ProcessingStep.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessingStep')

## ProcessingStep.EnableContinuation() Method

Activate continuation for this activity. While in the context that is enabling continuation, this activity can
still be updated and MUST be ended with a call to EndProcessingStepActivity().

```csharp
public string EnableContinuation();
```

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')