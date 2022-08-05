#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Scheduling](Be.Stateless.BizTalk.Dsl.Binding.Scheduling.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling')

## WeeklyServiceWindow Class

Scheduling properties for a receive location.

```csharp
public class WeeklyServiceWindow : Be.Stateless.BizTalk.Dsl.Binding.Scheduling.RecurringServiceWindow
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [ServiceWindow](ServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.ServiceWindow') &#129106; [RecurringServiceWindow](RecurringServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.RecurringServiceWindow') &#129106; WeeklyServiceWindow

### See Also
- [Configure scheduling for a receive location](https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-scheduling-for-a-receive-location#configure-scheduling-for-a-receive-location 'https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-scheduling-for-a-receive-location#configure-scheduling-for-a-receive-location')

| Constructors | |
| :--- | :--- |
| [WeeklyServiceWindow()](WeeklyServiceWindow.WeeklyServiceWindow().md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.WeeklyServiceWindow.WeeklyServiceWindow()') | |

| Properties | |
| :--- | :--- |
| [From](WeeklyServiceWindow.From.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.WeeklyServiceWindow.From') | The [System.DateTime](https://docs.microsoft.com/en-us/dotnet/api/System.DateTime 'System.DateTime') on which the [WeeklyServiceWindow](WeeklyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.WeeklyServiceWindow') recurrence starts. |
| [Interval](WeeklyServiceWindow.Interval.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.WeeklyServiceWindow.Interval') | Number of weeks between [WeeklyServiceWindow](WeeklyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.WeeklyServiceWindow') activations. |
| [WeekDays](WeeklyServiceWindow.WeekDays.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.WeeklyServiceWindow.WeekDays') | Days on which the [WeeklyServiceWindow](WeeklyServiceWindow.md 'Be.Stateless.BizTalk.Dsl.Binding.Scheduling.WeeklyServiceWindow') recurrence will be activated. |
