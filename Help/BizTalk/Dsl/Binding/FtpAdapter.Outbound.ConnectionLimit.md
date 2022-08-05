#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter').[Outbound](FtpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound')

## FtpAdapter.Outbound.ConnectionLimit Property

Specify the maximum number of concurrent FTP connections that can be opened to the server. A value of 0 means no
limit.

```csharp
public int ConnectionLimit { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks
It defaults to `0` seconds.