#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter').[Inbound](FtpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound')

## FtpAdapter.Inbound.PollingInterval Property

Specify the interval number for polling this location.

```csharp
public System.TimeSpan PollingInterval { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks

To poll continuously, set this value to zero (0).

It defaults to `60` seconds.