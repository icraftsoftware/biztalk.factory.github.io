#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter').[Inbound](FtpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound')

## FtpAdapter.Inbound.RedownloadInterval Property

Specify the interval after which the adapter downloads files again.

```csharp
public System.TimeSpan RedownloadInterval { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks

This property is applicable only when both [DeleteAfterDownload](FtpAdapter.Inbound.DeleteAfterDownload.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.DeleteAfterDownload') and [EnableTimestampComparison](FtpAdapter.Inbound.EnableTimestampComparison.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.EnableTimestampComparison') are set to `False`.

A negative [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan') indicates that the adapter will not download files again.

A zero [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan'), [System.TimeSpan.Zero](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan.Zero 'System.TimeSpan.Zero'), indicates that the adapter will download the file in
each polling cycle.

It defaults to a negative [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan').