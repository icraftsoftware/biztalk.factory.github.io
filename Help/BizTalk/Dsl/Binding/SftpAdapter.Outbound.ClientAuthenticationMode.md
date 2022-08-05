#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SftpAdapter](SftpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter').[Outbound](SftpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound')

## SftpAdapter.Outbound.ClientAuthenticationMode Property

Specifies the authentication method that the receive location uses for authenticating the client to the SSH
Server.

```csharp
public Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode ClientAuthenticationMode { get; set; }
```

#### Property Value
[Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode 'Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode')

### Remarks

If set to Password, you must specify the value in the [Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password 'Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password') property. If set to [Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.PublicKeyAuthentication](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.PublicKeyAuthentication 'Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.PublicKeyAuthentication'), you must specify the
private key of the user in the [PrivateKeyFile](SftpAdapter.Outbound.PrivateKeyFile.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.PrivateKeyFile') property. If set to [Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.MultiFactorAuthentication](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.MultiFactorAuthentication 'Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.MultiFactorAuthentication') you must provide [UserName](SftpAdapter.Outbound.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.UserName') with its [Password](SftpAdapter.Outbound.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.Password') and [PrivateKeyFile](SftpAdapter.Outbound.PrivateKeyFile.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.PrivateKeyFile'). Additionally, if the private
key is protected by a password, specify the password as well for the [PrivateKeyPassword](SftpAdapter.Outbound.PrivateKeyPassword.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.PrivateKeyPassword') property.

It defaults to [Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password 'Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password').