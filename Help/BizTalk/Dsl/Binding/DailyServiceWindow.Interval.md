#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Scheduling](Be.Stateless.BizTalk.Dsl.Binding.Scheduling.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling').[DailyServiceWindow](DailyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.DailyServiceWindow')

## DailyServiceWindow.Interval Property

Number of days between [DailyServiceWindow](DailyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.DailyServiceWindow') activations.

```csharp
public int Interval { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks
When configured a [DailyServiceWindow](DailyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.DailyServiceWindow') will recur every [Interval](DailyServiceWindow.Interval.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.DailyServiceWindow.Interval') days; from `1` to
`999`.