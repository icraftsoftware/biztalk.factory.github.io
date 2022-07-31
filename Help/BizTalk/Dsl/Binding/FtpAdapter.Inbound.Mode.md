#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter').[Inbound](FtpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound')

## FtpAdapter.Inbound.Mode Property

Specify the mode in which the adapter connects to the FTP server.

```csharp
public Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Mode Mode { get; set; }
```

#### Property Value
[Mode](FtpAdapter.Mode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Mode')

### Remarks

In active mode, the FTP server connects to a port opened by the FTP adapter. In passive mode, the FTP
adapter connects to a port opened by the FTP server.

It defaults to [Active](FtpAdapter.Mode.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Mode.Active 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Mode.Active');