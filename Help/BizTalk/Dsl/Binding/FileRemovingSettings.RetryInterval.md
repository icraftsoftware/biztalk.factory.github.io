#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FileRemovingSettings](FileRemovingSettings.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileRemovingSettings')

## FileRemovingSettings.RetryInterval Property

Removing of files retry interval.

```csharp
public System.TimeSpan RetryInterval { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks

Specify the initial interval that the file adapter waits before attempting to delete a file that it has read and
submitted to BizTalk Server. This interval will double after each retry interval up to the specified maximum retry
interval value.

See also File Transport Properties Dialog Box, Receive, Advanced Settings Dialog Box,
https://docs.microsoft.com/en-us/biztalk/core/technical-reference/file-transport-properties-dialog-box-receive-advanced-settings-dialog-box