#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SftpAdapter](SftpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter').[Inbound](SftpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound')

## SftpAdapter.Inbound.MaxConnectionReuseTime Property

The maximum connection reuse time allows connections to be gracefully closed and removed from the pool after a
connection has been in use for a specific amount of time.

```csharp
public System.TimeSpan MaxConnectionReuseTime { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks

A value of `0` or less indicates that this behaviour is disabled.

It defaults to `0`.