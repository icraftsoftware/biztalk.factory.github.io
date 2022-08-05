#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[Office365EmailAdapter](Office365EmailAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter').[Inbound](Office365EmailAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound')

## Office365EmailAdapter.Inbound.IncludeAttachments Property

Whether to retrieve email's attachments as parts of the BizTalk message.

```csharp
public bool IncludeAttachments { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

It is `false` by default.

Each BizTalk message part has the [Microsoft.BizTalk.Message.Interop.IBaseMessage](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage 'Microsoft.BizTalk.Message.Interop.IBaseMessage') ContentType property set to the `MIME` type of
the attachment. Attachments that are Outlook items (emails, calendar events, contacts) are saved in their
`MIME` representation.