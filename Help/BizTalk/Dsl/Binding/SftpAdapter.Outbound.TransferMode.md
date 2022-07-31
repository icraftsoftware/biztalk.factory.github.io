#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SftpAdapter](SftpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter').[Outbound](SftpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound')

## SftpAdapter.Outbound.TransferMode Property

Specify the transfer mode.

```csharp
public Microsoft.BizTalk.Adapter.Sftp.TransferMode TransferMode { get; set; }
```

#### Property Value
[Microsoft.BizTalk.Adapter.Sftp.TransferMode](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.TransferMode 'Microsoft.BizTalk.Adapter.Sftp.TransferMode')

### Remarks
When [TransferMode](SftpAdapter.Outbound.TransferMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.TransferMode') is set to [Microsoft.BizTalk.Adapter.Sftp.TransferMode.ASCII](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.TransferMode.ASCII 'Microsoft.BizTalk.Adapter.Sftp.TransferMode.ASCII'), it
allows to not only transfer but also to convert text files to the format used by the target platform.