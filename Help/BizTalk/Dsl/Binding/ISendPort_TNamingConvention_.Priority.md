#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding').[ISendPort&lt;TNamingConvention&gt;](ISendPort_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>')

## ISendPort<TNamingConvention>.Priority Property

Priority of the resend attempt.

```csharp
Be.Stateless.BizTalk.Dsl.Binding.Priority Priority { get; }
```

#### Property Value
[Priority](Priority.md 'Be.Stateless.BizTalk.Dsl.Binding.Priority')

### Remarks

Internally, BizTalk Server assigns a priority to every subscription. Priority can be any number from 1 ([Highest](Priority.md#Be.Stateless.BizTalk.Dsl.Binding.Priority.Highest 'Be.Stateless.BizTalk.Dsl.Binding.Priority.Highest') priority) to 10 ([Lowest](Priority.md#Be.Stateless.BizTalk.Dsl.Binding.Priority.Lowest 'Be.Stateless.BizTalk.Dsl.Binding.Priority.Lowest') priority). Because the
default priority is 7 for activating subscriptions and 5 for correlating subscriptions, correlating messages will be
delivered earlier than activating subscriptions.

See also:
- How to Configure Transport Advanced Options for a Send Port,
  https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-transport-advanced-options-for-a-send-port.