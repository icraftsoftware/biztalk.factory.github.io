#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[Office365EmailAdapter](Office365EmailAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter').[Inbound](Office365EmailAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound')

## Office365EmailAdapter.Inbound.FolderName Property

The folder to fetch emails from.

```csharp
public string FolderName { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
The default folder is `Inbox`. Note that folders are not recursive.