#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SftpAdapter](SftpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter').[Inbound](SftpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound')

## SftpAdapter.Inbound.AcceptAnySshServerHostKey Property

If set to `True`, the receive location accepts any SSH public host key from the server. If set to
`False`, the receive location uses the fingerprint of the server for authentication. You specify the
fingerprint in the [SshServerHostKeyFingerPrint](SftpAdapter.Inbound.SshServerHostKeyFingerPrint.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.SshServerHostKeyFingerPrint') property.

```csharp
public bool AcceptAnySshServerHostKey { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks
It defaults to `False`.