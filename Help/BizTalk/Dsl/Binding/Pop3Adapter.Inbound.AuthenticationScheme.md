#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[Pop3Adapter](Pop3Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter').[Inbound](Pop3Adapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound')

## Pop3Adapter.Inbound.AuthenticationScheme Property

Specify the type of authentication to use with the destination server.

```csharp
public Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.AuthenticationScheme AuthenticationScheme { get; set; }
```

#### Property Value
[AuthenticationScheme](Pop3Adapter.AuthenticationScheme.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.AuthenticationScheme')

### Remarks
Valid options are:
- [Basic](Pop3Adapter.AuthenticationScheme.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.AuthenticationScheme.Basic 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.AuthenticationScheme.Basic') — Password will be sent to POP3 server in clear text.
- [Digest](Pop3Adapter.AuthenticationScheme.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.AuthenticationScheme.Digest 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.AuthenticationScheme.Digest') — Password hash will be sent to POP3 server.
- [SecurePasswordAuthentication](Pop3Adapter.AuthenticationScheme.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.AuthenticationScheme.SecurePasswordAuthentication 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.AuthenticationScheme.SecurePasswordAuthentication') — NTLM will be used for authentication. The username must be specified with one of the following formats:
  - Domain accounts must be entered with the syntax: `<domain name>\<username>`.
  - Local accounts must be entered with the syntax: `<machine name>\<username>`.