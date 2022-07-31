#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SBMessagingAdapter&lt;TConfig&gt;](SBMessagingAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>')

## SBMessagingAdapter<TConfig>.OpenTimeout Property

Specifies a timespan value that indicates the time for a channel open operation to complete.

```csharp
public System.TimeSpan OpenTimeout { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks
It defaults to `1` minute.