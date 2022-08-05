#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter').[Outbound](FtpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound')

## FtpAdapter.Outbound.TemporaryFolder Property

Specify the location for a temporary folder.

```csharp
public string TemporaryFolder { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
The file is first uploaded here and then moved to the destination FTP folder. In case of transfer failure, the
adapter restarts the file upload in ASCII mode of transfer and resumes in binary mode of transfer.