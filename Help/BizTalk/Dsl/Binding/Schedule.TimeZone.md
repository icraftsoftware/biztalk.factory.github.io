#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Scheduling](Be.Stateless.BizTalk.Dsl.Binding.Scheduling.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling').[Schedule](Schedule.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule')

## Schedule.TimeZone Property

The [TimeZone](Schedule.TimeZone.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.TimeZone') determines all the date time values of the [Schedule](Schedule.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule') and its [ServiceWindow](Schedule.ServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.ServiceWindow') or any of its derived [ServiceWindow](Schedule.ServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.ServiceWindow').

```csharp
public System.TimeZoneInfo TimeZone { get; set; }
```

#### Property Value
[System.TimeZoneInfo](https://docs.microsoft.com/en-us/dotnet/api/System.TimeZoneInfo 'System.TimeZoneInfo')

### See Also
- [DailyServiceWindow](DailyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.DailyServiceWindow')
- [WeeklyServiceWindow](WeeklyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.WeeklyServiceWindow')
- [CalendricalMonthlyServiceWindow](CalendricalMonthlyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.CalendricalMonthlyServiceWindow')
- [OrdinalMonthlyServiceWindow](OrdinalMonthlyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.OrdinalMonthlyServiceWindow')