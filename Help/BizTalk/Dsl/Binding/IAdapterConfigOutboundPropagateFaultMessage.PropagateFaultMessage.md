#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigOutboundPropagateFaultMessage](IAdapterConfigOutboundPropagateFaultMessage.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundPropagateFaultMessage')

## IAdapterConfigOutboundPropagateFaultMessage.PropagateFaultMessage Property

Specify whether to route or suspend messages failed in outbound processing.

```csharp
bool PropagateFaultMessage { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

- `True` — Route the message that fails outbound processing to a subscribing application (such as another
              receive port or orchestration schedule).
- `False` — Suspend failed messages and generate a negative acknowledgment (NACK).

This property is valid only for solicit-response ports.

It defaults to `True`.