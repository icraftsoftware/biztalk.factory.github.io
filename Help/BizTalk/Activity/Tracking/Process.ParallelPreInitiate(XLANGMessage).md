#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Tracking.Processing](Be.Stateless.BizTalk.Activity.Tracking.Processing.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing').[Process](Process.md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process')

## Process.ParallelPreInitiate(XLANGMessage) Method

Method intended to be called at the start of an orchestration immediately after each one of its activating parallel
receives.

```csharp
public static void ParallelPreInitiate(Microsoft.XLANGs.BaseTypes.XLANGMessage activatingMessage);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.ParallelPreInitiate(Microsoft.XLANGs.BaseTypes.XLANGMessage).activatingMessage'></a>

`activatingMessage` [Microsoft.XLANGs.BaseTypes.XLANGMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.XLANGMessage 'Microsoft.XLANGs.BaseTypes.XLANGMessage')

The message that activates the orchestration instance.

### Remarks
Notice that no BAM process tracking activity will be created. Instead, the activating message will be associated
ahead of time to its forthcoming BAM process activity, see [ParallelInitiate()](Process.ParallelInitiate().md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.ParallelInitiate()') and [ParallelInitiate(XLANGMessage)](Process.ParallelInitiate(XLANGMessage).md 'Be.Stateless.BizTalk.Activity.Tracking.Processing.Process.ParallelInitiate(Microsoft.XLANGs.BaseTypes.XLANGMessage)').