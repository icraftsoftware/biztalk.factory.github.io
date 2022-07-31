#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[Pop3Adapter](Pop3Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter')

## Pop3Adapter.AuthenticationScheme Enum

```csharp
public enum Pop3Adapter.AuthenticationScheme
```
### Fields

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.AuthenticationScheme.Basic'></a>

`Basic` 0

Password will be sent to POP3 server in clear text.

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.AuthenticationScheme.Digest'></a>

`Digest` 1

Password hash will be sent to POP3 server.

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.AuthenticationScheme.SecurePasswordAuthentication'></a>

`SecurePasswordAuthentication` 2

NTLM will be used for authentication.