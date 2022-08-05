#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Scheduling](Be.Stateless.BizTalk.Dsl.Binding.Scheduling.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling').[WeeklyServiceWindow](WeeklyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.WeeklyServiceWindow')

## WeeklyServiceWindow.Interval Property

Number of weeks between [WeeklyServiceWindow](WeeklyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.WeeklyServiceWindow') activations.

```csharp
public int Interval { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks
When configured a [WeeklyServiceWindow](WeeklyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.WeeklyServiceWindow') will recur every [Interval](WeeklyServiceWindow.Interval.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.WeeklyServiceWindow.Interval') weeks; from `1` to
`999`.