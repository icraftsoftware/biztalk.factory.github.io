#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FileRemovingSettings](FileRemovingSettings.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileRemovingSettings')

## FileRemovingSettings.MaxRetryInterval Property

Removing of files retry interval.

```csharp
public System.TimeSpan MaxRetryInterval { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks

Specify the maximum retry interval time that the file adapter waits before attempting to delete a file that it has
read and submitted to BizTalk Server.

See also File Transport Properties Dialog Box, Receive, Advanced Settings Dialog Box,
https://docs.microsoft.com/en-us/biztalk/core/technical-reference/file-transport-properties-dialog-box-receive-advanced-settings-dialog-box