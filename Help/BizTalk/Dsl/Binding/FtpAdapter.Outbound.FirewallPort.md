#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter').[Outbound](FtpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound')

## FtpAdapter.Outbound.FirewallPort Property

Specify the port for the firewall.

```csharp
public uint FirewallPort { get; set; }
```

#### Property Value
[System.UInt32](https://docs.microsoft.com/en-us/dotnet/api/System.UInt32 'System.UInt32')

### Remarks

Values range from `1` to `65535`.

It defaults to `21`.