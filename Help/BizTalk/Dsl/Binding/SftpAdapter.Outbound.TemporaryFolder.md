#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SftpAdapter](SftpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter').[Outbound](SftpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound')

## SftpAdapter.Outbound.TemporaryFolder Property

A temporary folder on the SFTP server to upload large files to, before they can be atomically moved to the
required location on the same server.

```csharp
public string TemporaryFolder { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')