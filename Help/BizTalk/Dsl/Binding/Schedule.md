#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Scheduling](Be.Stateless.BizTalk.Dsl.Binding.Scheduling.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling')

## Schedule Class

Scheduling properties for a receive location.

```csharp
public class Schedule
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; Schedule

### See Also
- [Configure scheduling for a receive location](https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-scheduling-for-a-receive-location#configure-scheduling-for-a-receive-location 'https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-scheduling-for-a-receive-location#configure-scheduling-for-a-receive-location')

| Constructors | |
| :--- | :--- |
| [Schedule()](Schedule.Schedule().md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.Schedule()') | |

| Properties | |
| :--- | :--- |
| [AutomaticallyAdjustForDaylightSavingTime](Schedule.AutomaticallyAdjustForDaylightSavingTime.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.AutomaticallyAdjustForDaylightSavingTime') | The [Schedule](Schedule.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule') automatically adjusts to the daylight saving time of the time zone you chose. |
| [None](Schedule.None.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.None') | |
| [RecurrenceType](Schedule.RecurrenceType.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.RecurrenceType') | |
| [ServiceWindow](Schedule.ServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.ServiceWindow') | Any [RecurringServiceWindow](RecurringServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.RecurringServiceWindow')-derived service window restricts the [ReceiveLocationBase&lt;TNamingConvention&gt;](ReceiveLocationBase_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>') to work during certain hours of the day possibly at a recurring period of time. |
| [StartDate](Schedule.StartDate.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.StartDate') | |
| [StartDateEnabled](Schedule.StartDateEnabled.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.StartDateEnabled') | |
| [StopDate](Schedule.StopDate.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.StopDate') | |
| [StopDateEnabled](Schedule.StopDateEnabled.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.StopDateEnabled') | |
| [TimeZone](Schedule.TimeZone.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.TimeZone') | The [TimeZone](Schedule.TimeZone.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.TimeZone') determines all the date time values of the [Schedule](Schedule.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule') and its [ServiceWindow](Schedule.ServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.ServiceWindow') or any of its derived [ServiceWindow](Schedule.ServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule.ServiceWindow'). |
