#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Scheduling](Be.Stateless.BizTalk.Dsl.Binding.Scheduling.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling').[Schedule](Schedule.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule')

## Schedule.AutomaticallyAdjustForDaylightSavingTime Property

The [Schedule](Schedule.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule') automatically adjusts to the daylight saving time of the time zone you chose.

```csharp
public bool AutomaticallyAdjustForDaylightSavingTime { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks
This option has no impact on the schedule if the time zone you chose doesn't have a daylight savings time, or
daylight savings time isn't observed