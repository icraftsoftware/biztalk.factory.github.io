#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SftpAdapter](SftpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter').[Inbound](SftpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound')

## SftpAdapter.Inbound.RedownloadInterval Property

The interval after which the file will be downloaded again. Applicable if [RetainAfterDownload](SftpAdapter.Inbound.RetainAfterDownload.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.RetainAfterDownload') is
`True`, and [EnableTimeComparison](SftpAdapter.Inbound.EnableTimeComparison.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.EnableTimeComparison') is `False`. If set to -1, the file will not be downloaded
again.

```csharp
public int RedownloadInterval { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks

It defaults to `0`.

- `-1` indicates that the adapter will not download files again.
- `0` indicates that the adapter will download the file in each polling cycle.