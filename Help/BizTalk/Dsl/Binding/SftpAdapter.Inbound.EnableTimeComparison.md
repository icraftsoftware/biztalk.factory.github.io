#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SftpAdapter](SftpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter').[Inbound](SftpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound')

## SftpAdapter.Inbound.EnableTimeComparison Property

If [RetainAfterDownload](SftpAdapter.Inbound.RetainAfterDownload.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.RetainAfterDownload') is set to `True`, this property determines whether a change in file
timestamp will trigger a redownload of the file.

```csharp
public bool EnableTimeComparison { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks
It defaults to `False`.