#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[Pop3Adapter](Pop3Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter').[Inbound](Pop3Adapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound')

## Pop3Adapter.Inbound.PollingInterval Property

Specify the interval between attempts to retrieve messages from the POP3 server.

```csharp
public System.TimeSpan PollingInterval { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks
It defaults to `5` minutes.