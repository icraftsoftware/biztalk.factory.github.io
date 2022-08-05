#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Scheduling](Be.Stateless.BizTalk.Dsl.Binding.Scheduling.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling').[Schedule](Schedule.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.Schedule')

## Schedule.ServiceWindow Property

Any [RecurringServiceWindow](RecurringServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.RecurringServiceWindow')-derived service window restricts the [ReceiveLocationBase&lt;TNamingConvention&gt;](ReceiveLocationBase_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.ReceiveLocationBase<TNamingConvention>') to work during certain hours of the day possibly at a recurring
period of time.

```csharp
public Be.Stateless.BizTalk.Dsl.Binding.Scheduling.RecurringServiceWindow ServiceWindow { get; set; }
```

#### Property Value
[RecurringServiceWindow](RecurringServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.RecurringServiceWindow')

### See Also
- [DailyServiceWindow](DailyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.DailyServiceWindow')
- [WeeklyServiceWindow](WeeklyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.WeeklyServiceWindow')
- [CalendricalMonthlyServiceWindow](CalendricalMonthlyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.CalendricalMonthlyServiceWindow')
- [OrdinalMonthlyServiceWindow](OrdinalMonthlyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.OrdinalMonthlyServiceWindow')