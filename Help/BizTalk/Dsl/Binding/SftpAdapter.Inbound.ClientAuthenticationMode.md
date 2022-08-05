#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SftpAdapter](SftpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter').[Inbound](SftpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound')

## SftpAdapter.Inbound.ClientAuthenticationMode Property

Specifies the authentication method that the receive location uses for authenticating the client to the SSH
Server.

```csharp
public Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode ClientAuthenticationMode { get; set; }
```

#### Property Value
[Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode 'Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode')

### Remarks

If set to Password, you must specify the value in the [Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password 'Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password') property. If set to [Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.PublicKeyAuthentication](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.PublicKeyAuthentication 'Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.PublicKeyAuthentication'), you must specify the
private key of the user in the [PrivateKeyFile](SftpAdapter.Inbound.PrivateKeyFile.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.PrivateKeyFile') property. If set to [Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.MultiFactorAuthentication](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.MultiFactorAuthentication 'Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.MultiFactorAuthentication') you must provide [UserName](SftpAdapter.Inbound.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.UserName') with its [Password](SftpAdapter.Inbound.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.Password') and [PrivateKeyFile](SftpAdapter.Inbound.PrivateKeyFile.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.PrivateKeyFile'). Additionally, if the private
key is protected by a password, specify the password as well for the [PrivateKeyPassword](SftpAdapter.Inbound.PrivateKeyPassword.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.PrivateKeyPassword') property.

It defaults to [Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password 'Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password').