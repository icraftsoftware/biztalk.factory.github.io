#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[Pop3Adapter](Pop3Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter').[Inbound](Pop3Adapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound')

## Pop3Adapter.Inbound.Port Property

Specify the port for the POP3 mail server.

```csharp
public int Port { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks

Valid values ranges from `0` to `65535` inclusive.

It defaults to `0`.

A value of `0` indicates to use the default POP3 port of `110` if [UseSsl](Pop3Adapter.Inbound.UseSsl.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.UseSsl') is `False`
or port `995` if [UseSsl](Pop3Adapter.Inbound.UseSsl.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.UseSsl') is `True`.