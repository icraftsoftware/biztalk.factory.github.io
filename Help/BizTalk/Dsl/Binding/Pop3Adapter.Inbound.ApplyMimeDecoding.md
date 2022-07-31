#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[Pop3Adapter](Pop3Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter').[Inbound](Pop3Adapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound')

## Pop3Adapter.Inbound.ApplyMimeDecoding Property

Specify whether to apply MIME decoding to messages received by the POP3 adapter. MIME decoding is used to parse
the incoming message and any attachments into a multi-part BizTalk message.

```csharp
public bool ApplyMimeDecoding { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

If this value is set to `False` then the POP3 adapter will submit the complete e-mail body including message
headers to BizTalk Server.

It defaults to `True`.