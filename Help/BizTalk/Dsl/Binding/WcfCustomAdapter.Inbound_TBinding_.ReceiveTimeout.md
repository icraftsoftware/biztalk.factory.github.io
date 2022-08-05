#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfCustomAdapter](WcfCustomAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter').[Inbound&lt;TBinding&gt;](WcfCustomAdapter.Inbound_TBinding_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>')

## WcfCustomAdapter.Inbound<TBinding>.ReceiveTimeout Property

On the service side, initialize the session-idle timeout which controls how long a session can be idle before
timing out.

```csharp
public System.TimeSpan ReceiveTimeout { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks
It defaults to `10` minutes.