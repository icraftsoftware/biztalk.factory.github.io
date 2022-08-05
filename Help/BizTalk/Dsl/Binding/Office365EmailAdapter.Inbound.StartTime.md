#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[Office365EmailAdapter](Office365EmailAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter').[Inbound](Office365EmailAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound')

## Office365EmailAdapter.Inbound.StartTime Property

The minimum received TimeStamp of an email in Office 365 Outlook.

```csharp
public System.DateTimeOffset StartTime { get; set; }
```

#### Property Value
[System.DateTimeOffset](https://docs.microsoft.com/en-us/dotnet/api/System.DateTimeOffset 'System.DateTimeOffset')

### Remarks
Only emails more recent than the entered values will be received.