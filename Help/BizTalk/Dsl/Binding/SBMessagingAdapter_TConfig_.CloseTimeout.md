#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SBMessagingAdapter&lt;TConfig&gt;](SBMessagingAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>')

## SBMessagingAdapter<TConfig>.CloseTimeout Property

Specifies a timespan value that indicates the time for a channel close operation to complete.

```csharp
public System.TimeSpan CloseTimeout { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks
It defaults to `1` minute.