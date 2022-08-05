#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter').[Outbound](FtpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound')

## FtpAdapter.Outbound.UseDataProtection Property

Specify if the adapter must use SSL encryption or plain text when it sends and receives data files from the FTPS
server.

```csharp
public Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Boolean UseDataProtection { get; set; }
```

#### Property Value
[Boolean](FtpAdapter.Boolean.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Boolean')

### Remarks
It defaults to `True`.