#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter').[Inbound](FtpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound')

## FtpAdapter.Inbound.EnableTimestampComparison Property

Specify whether the adapter downloads a file again based on its modified timestamp. In cases when the adapter does
not have delete permissions on the FTP server, the MDTM (Modification Time) command allows the adapter to know
whether a file has been modified since last download. Based on the value of this property, the file is downloaded
again.

```csharp
public Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Boolean EnableTimestampComparison { get; set; }
```

#### Property Value
[Boolean](FtpAdapter.Boolean.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Boolean')

### Remarks

In case the FTP server does not support MDTM, set the [RedownloadInterval](FtpAdapter.Inbound.RedownloadInterval.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.RedownloadInterval') property.

This property is applicable only when [DeleteAfterDownload](FtpAdapter.Inbound.DeleteAfterDownload.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.DeleteAfterDownload') is set to `False`.

It defaults to `False`.