#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SftpAdapter](SftpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter').[Outbound](SftpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound')

## SftpAdapter.Outbound.SshServerHostKeyFingerPrint Property

Specifies the fingerprint of the server used by the adapter to authenticate the server if the [AcceptAnySshServerHostKey](SftpAdapter.Outbound.AcceptAnySshServerHostKey.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.AcceptAnySshServerHostKey') property is set to `False`. If the fingerprints do not match, the
connection fails.

```csharp
public string SshServerHostKeyFingerPrint { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')