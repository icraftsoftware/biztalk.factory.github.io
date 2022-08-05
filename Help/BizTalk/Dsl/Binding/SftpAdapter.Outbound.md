#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SftpAdapter](SftpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter')

## SftpAdapter.Outbound Class

Use the SFTP adapter to send and receive messages from a secure FTP server using the SSH file transfer protocol.

```csharp
public class SftpAdapter.Outbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter<Microsoft.BizTalk.Adapter.Sftp.SftpTLConfig>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IOutboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter&lt;](SftpAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter<TConfig>')[Microsoft.BizTalk.Adapter.Sftp.SftpTLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.SftpTLConfig 'Microsoft.BizTalk.Adapter.Sftp.SftpTLConfig')[&gt;](SftpAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter<TConfig>') &#129106; Outbound

Implements [IOutboundAdapter](IOutboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IOutboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation')

### See Also
- [SFTP Adapter](https://docs.microsoft.com/en-us/biztalk/core/sftp-adapter 'https://docs.microsoft.com/en-us/biztalk/core/sftp-adapter')
- [Configure the send port](https://docs.microsoft.com/en-us/biztalk/core/sftp-adapter#configure-the-send-port 'https://docs.microsoft.com/en-us/biztalk/core/sftp-adapter#configure-the-send-port')
- [Frequently asked questions](https://docs.microsoft.com/en-us/biztalk/core/sftp-adapter#frequently-asked-questions 'https://docs.microsoft.com/en-us/biztalk/core/sftp-adapter#frequently-asked-questions')

| Constructors | |
| :--- | :--- |
| [Outbound()](SftpAdapter.Outbound.Outbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.Outbound()') | |
| [Outbound(Action&lt;Outbound&gt;)](SftpAdapter.Outbound.Outbound(Action_Outbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.Outbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound>)') | |

| Properties | |
| :--- | :--- |
| [AcceptAnySshServerHostKey](SftpAdapter.Outbound.AcceptAnySshServerHostKey.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.AcceptAnySshServerHostKey') | If set to `True`, the receive location accepts any SSH public host key from the server. If set to `False`, the receive location uses the fingerprint of the server for authentication. You specify the fingerprint in the [SshServerHostKeyFingerPrint](SftpAdapter.Outbound.SshServerHostKeyFingerPrint.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.SshServerHostKeyFingerPrint') property. |
| [AffiliateApplicationName](SftpAdapter.Outbound.AffiliateApplicationName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.AffiliateApplicationName') | The Single Sign On (SSO) Affiliate Application. |
| [AppendIfExists](SftpAdapter.Outbound.AppendIfExists.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.AppendIfExists') | If the file being transferred to the secure FTP server already exists at the destination, this property specifies whether the data from the file being transferred should be appended to the existing file. If set to `True`, the data is appended. If set to `False`, the file at the destination server is overwritten. |
| [ClientAuthenticationMode](SftpAdapter.Outbound.ClientAuthenticationMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.ClientAuthenticationMode') | Specifies the authentication method that the receive location uses for authenticating the client to the SSH Server. |
| [ConnectionLimit](SftpAdapter.Outbound.ConnectionLimit.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.ConnectionLimit') | Specify the maximum number of concurrent connections that can be opened to the server. |
| [EncryptionCipher](SftpAdapter.Outbound.EncryptionCipher.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.EncryptionCipher') | Specify the kind of encryption cipher. |
| [FolderPath](SftpAdapter.Outbound.FolderPath.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.FolderPath') | Specifies the folder path on the secure FTP server where the file is copied. |
| [KeyExchangeAlgorithmSelectionPolicy](SftpAdapter.Outbound.KeyExchangeAlgorithmSelectionPolicy.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.KeyExchangeAlgorithmSelectionPolicy') | Comma-separated list of KEX preference order. Token WARN is used to delimit substandard KEXes. Example: ecdh,dh-gex-sha1,dh-group14-sha1,rsa,WARN,dh-group1-sha1. Visit WinSCP website for latest information. |
| [Log](SftpAdapter.Outbound.Log.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.Log') | The full path to create a client-side log file. Use this log file to troubleshoot any errors. |
| [MaxConnectionReuseTime](SftpAdapter.Outbound.MaxConnectionReuseTime.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.MaxConnectionReuseTime') | The maximum connection reuse time allows connections to be gracefully closed and removed from the pool after a connection has been in use for a specific amount of time. |
| [Password](SftpAdapter.Outbound.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.Password') | Specify the SFTP user password if you set the [ClientAuthenticationMode](SftpAdapter.Outbound.ClientAuthenticationMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.ClientAuthenticationMode') to [Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password 'Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password'). |
| [Port](SftpAdapter.Outbound.Port.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.Port') | Specifies the port address for the secure FTP server on which the file transfer takes place. |
| [PrivateKeyFile](SftpAdapter.Outbound.PrivateKeyFile.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.PrivateKeyFile') | Specify the private key for the SFTP user if you set the [ClientAuthenticationMode](SftpAdapter.Outbound.ClientAuthenticationMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.ClientAuthenticationMode') to [Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.PublicKeyAuthentication](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.PublicKeyAuthentication 'Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.PublicKeyAuthentication'). |
| [PrivateKeyPassword](SftpAdapter.Outbound.PrivateKeyPassword.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.PrivateKeyPassword') | Specify a private key password, if required for the key specified in the [PrivateKeyFile](SftpAdapter.Outbound.PrivateKeyFile.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.PrivateKeyFile') property. |
| [ProxyAddress](SftpAdapter.Outbound.ProxyAddress.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.ProxyAddress') | Specifies either the DNS name or the IP address of the proxy server. |
| [ProxyPassword](SftpAdapter.Outbound.ProxyPassword.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.ProxyPassword') | Specifies the password for the proxy server. |
| [ProxyPort](SftpAdapter.Outbound.ProxyPort.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.ProxyPort') | Specifies the port for the proxy server. |
| [ProxyType](SftpAdapter.Outbound.ProxyType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.ProxyType') | Specifies the protocol used by the proxy server. |
| [ProxyUserName](SftpAdapter.Outbound.ProxyUserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.ProxyUserName') | Specifies the username for the proxy server. |
| [ServerAddress](SftpAdapter.Outbound.ServerAddress.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.ServerAddress') | Specifies the server name or IP address of the secure FTP server. |
| [SshServerHostKeyFingerPrint](SftpAdapter.Outbound.SshServerHostKeyFingerPrint.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.SshServerHostKeyFingerPrint') | Specifies the fingerprint of the server used by the adapter to authenticate the server if the [AcceptAnySshServerHostKey](SftpAdapter.Outbound.AcceptAnySshServerHostKey.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.AcceptAnySshServerHostKey') property is set to `False`. If the fingerprints do not match, the connection fails. |
| [TargetFileName](SftpAdapter.Outbound.TargetFileName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.TargetFileName') | Specifies the name with which the file is transferred to the secure FTP server. You can also use macros for the target file name. |
| [TemporaryFolder](SftpAdapter.Outbound.TemporaryFolder.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.TemporaryFolder') | A temporary folder on the SFTP server to upload large files to, before they can be atomically moved to the required location on the same server. |
| [TransferMode](SftpAdapter.Outbound.TransferMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.TransferMode') | Specify the transfer mode. |
| [UserName](SftpAdapter.Outbound.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.UserName') | Specifies a username to log on to the SFTP server. |

| Methods | |
| :--- | :--- |
| [GetAddress()](SftpAdapter.Outbound.GetAddress().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.GetAddress()') | |
| [Validate()](SftpAdapter.Outbound.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound.Validate()') | |
