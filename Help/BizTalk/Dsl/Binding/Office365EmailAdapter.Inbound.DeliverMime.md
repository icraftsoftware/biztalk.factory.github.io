#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[Office365EmailAdapter](Office365EmailAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter').[Inbound](Office365EmailAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound')

## Office365EmailAdapter.Inbound.DeliverMime Property

`true` to fetch an email in its raw `MIME` representation or `false` to process its content, i.e.
            to fetch its `MIME`-decoded body instead.

```csharp
public bool DeliverMime { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

It defaults to `false`.

When fetched in its raw `MIME` representation, the BizTalk message's content naturally includes email body
and all attachments.

When its content is processed while being fetched, the BizTalk message's content includes the email body and its
ContentType property is set to content type of the email body.

### See Also
- [IncludeAttachments](Office365EmailAdapter.Inbound.IncludeAttachments.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound.IncludeAttachments')