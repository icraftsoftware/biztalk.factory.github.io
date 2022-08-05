#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FileRemovingSettings](FileRemovingSettings.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileRemovingSettings')

## FileRemovingSettings.RetryCount Property

Removing of files retry count.

```csharp
public uint RetryCount { get; set; }
```

#### Property Value
[System.UInt32](https://docs.microsoft.com/en-us/dotnet/api/System.UInt32 'System.UInt32')

### Remarks

Specify the number of times that the file adapter will attempt to delete a file that it has read and submitted to
BizTalk Server.

See also File Transport Properties Dialog Box, Receive, Advanced Settings Dialog Box,
https://docs.microsoft.com/en-us/biztalk/core/technical-reference/file-transport-properties-dialog-box-receive-advanced-settings-dialog-box