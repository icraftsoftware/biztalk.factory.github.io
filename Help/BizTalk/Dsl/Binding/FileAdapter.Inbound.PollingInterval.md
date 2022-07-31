#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FileAdapter](FileAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter').[Inbound](FileAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound')

## FileAdapter.Inbound.PollingInterval Property

Receive location polling interval.

```csharp
public System.TimeSpan PollingInterval { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks

Specify the interval frequency that the file adapter will use to poll the specified location for new files; see
also <a href="https://docs.microsoft.com/en-us/biztalk/core/technical-reference/file-transport-properties-dialog-box-receive-advanced-settings-dialog-box">File
Transport Properties Dialog Box, Receive, Advanced Settings Dialog Box</a>.