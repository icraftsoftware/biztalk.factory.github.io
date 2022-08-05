#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SftpAdapter](SftpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter')

## SftpAdapter.Inbound Class

Use the SFTP adapter to send and receive messages from a secure FTP server using the SSH file transfer protocol.

```csharp
public class SftpAdapter.Inbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter<Microsoft.BizTalk.Adapter.Sftp.SftpRLConfig>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter&lt;](SftpAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter<TConfig>')[Microsoft.BizTalk.Adapter.Sftp.SftpRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.SftpRLConfig 'Microsoft.BizTalk.Adapter.Sftp.SftpRLConfig')[&gt;](SftpAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter<TConfig>') &#129106; Inbound

Implements [IInboundAdapter](IInboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation')

### See Also
- [SFTP Adapter](https://docs.microsoft.com/en-us/biztalk/core/sftp-adapter 'https://docs.microsoft.com/en-us/biztalk/core/sftp-adapter')
- [Configure the receive location](https://docs.microsoft.com/en-us/biztalk/core/sftp-adapter#configure-the-receive-location 'https://docs.microsoft.com/en-us/biztalk/core/sftp-adapter#configure-the-receive-location')
- [Frequently asked questions](https://docs.microsoft.com/en-us/biztalk/core/sftp-adapter#frequently-asked-questions 'https://docs.microsoft.com/en-us/biztalk/core/sftp-adapter#frequently-asked-questions')

| Constructors | |
| :--- | :--- |
| [Inbound()](SftpAdapter.Inbound.Inbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.Inbound()') | |
| [Inbound(Action&lt;Inbound&gt;)](SftpAdapter.Inbound.Inbound(Action_Inbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.Inbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound>)') | |

| Properties | |
| :--- | :--- |
| [AcceptAnySshServerHostKey](SftpAdapter.Inbound.AcceptAnySshServerHostKey.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.AcceptAnySshServerHostKey') | If set to `True`, the receive location accepts any SSH public host key from the server. If set to `False`, the receive location uses the fingerprint of the server for authentication. You specify the fingerprint in the [SshServerHostKeyFingerPrint](SftpAdapter.Inbound.SshServerHostKeyFingerPrint.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.SshServerHostKeyFingerPrint') property. |
| [AffiliateApplicationName](SftpAdapter.Inbound.AffiliateApplicationName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.AffiliateApplicationName') | The Single Sign On (SSO) Affiliate Application. |
| [ClientAuthenticationMode](SftpAdapter.Inbound.ClientAuthenticationMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.ClientAuthenticationMode') | Specifies the authentication method that the receive location uses for authenticating the client to the SSH Server. |
| [ConnectionLimit](SftpAdapter.Inbound.ConnectionLimit.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.ConnectionLimit') | Specify the maximum number of concurrent connections that can be opened to the server. |
| [EnableTimeComparison](SftpAdapter.Inbound.EnableTimeComparison.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.EnableTimeComparison') | If [RetainAfterDownload](SftpAdapter.Inbound.RetainAfterDownload.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.RetainAfterDownload') is set to `True`, this property determines whether a change in file timestamp will trigger a redownload of the file. |
| [EncryptionCipher](SftpAdapter.Inbound.EncryptionCipher.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.EncryptionCipher') | Specify the kind of encryption cipher. |
| [FileMask](SftpAdapter.Inbound.FileMask.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.FileMask') | Specifies the file mask to use when retrieving files from a secure FTP server. |
| [FolderPath](SftpAdapter.Inbound.FolderPath.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.FolderPath') | Specifies the folder path on the secure FTP server from where the receive location can retrieve files. |
| [KeyExchangeAlgorithmSelectionPolicy](SftpAdapter.Inbound.KeyExchangeAlgorithmSelectionPolicy.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.KeyExchangeAlgorithmSelectionPolicy') | Comma-separated list of KEX preference order. Token WARN is used to delimit substandard KEXes. Example: ecdh,dh-gex-sha1,dh-group14-sha1,rsa,WARN,dh-group1-sha1. Visit WinSCP website for latest information. |
| [Log](SftpAdapter.Inbound.Log.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.Log') | The full path to create a client-side log file. Use this log file to troubleshoot any errors. |
| [MaxConnectionReuseTime](SftpAdapter.Inbound.MaxConnectionReuseTime.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.MaxConnectionReuseTime') | The maximum connection reuse time allows connections to be gracefully closed and removed from the pool after a connection has been in use for a specific amount of time. |
| [Password](SftpAdapter.Inbound.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.Password') | Specify the SFTP user password if you set the [ClientAuthenticationMode](SftpAdapter.Inbound.ClientAuthenticationMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.ClientAuthenticationMode') to [Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password 'Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.Password'). |
| [PollingInterval](SftpAdapter.Inbound.PollingInterval.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.PollingInterval') | Specify the intervals at which the adapter will poll the server. |
| [Port](SftpAdapter.Inbound.Port.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.Port') | Specifies the port address for the secure FTP server on which the file transfer takes place. |
| [PrivateKeyFile](SftpAdapter.Inbound.PrivateKeyFile.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.PrivateKeyFile') | Specify the private key for the SFTP user if you set the [ClientAuthenticationMode](SftpAdapter.Inbound.ClientAuthenticationMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.ClientAuthenticationMode') to [Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.PublicKeyAuthentication](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.PublicKeyAuthentication 'Microsoft.BizTalk.Adapter.Sftp.ClientAuthenticationMode.PublicKeyAuthentication'). |
| [PrivateKeyPassword](SftpAdapter.Inbound.PrivateKeyPassword.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.PrivateKeyPassword') | Specify a private key password, if required for the key specified in the [PrivateKeyFile](SftpAdapter.Inbound.PrivateKeyFile.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.PrivateKeyFile') property. |
| [ProxyAddress](SftpAdapter.Inbound.ProxyAddress.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.ProxyAddress') | Specifies either the DNS name or the IP address of the proxy server. |
| [ProxyPassword](SftpAdapter.Inbound.ProxyPassword.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.ProxyPassword') | Specifies the password for the proxy server. |
| [ProxyPort](SftpAdapter.Inbound.ProxyPort.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.ProxyPort') | Specifies the port for the proxy server. |
| [ProxyType](SftpAdapter.Inbound.ProxyType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.ProxyType') | Specifies the protocol used by the proxy server. |
| [ProxyUserName](SftpAdapter.Inbound.ProxyUserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.ProxyUserName') | Specifies the username for the proxy server. |
| [RedownloadInterval](SftpAdapter.Inbound.RedownloadInterval.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.RedownloadInterval') | The interval after which the file will be downloaded again. Applicable if [RetainAfterDownload](SftpAdapter.Inbound.RetainAfterDownload.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.RetainAfterDownload') is `True`, and [EnableTimeComparison](SftpAdapter.Inbound.EnableTimeComparison.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.EnableTimeComparison') is `False`. If set to -1, the file will not be downloaded again. |
| [RetainAfterDownload](SftpAdapter.Inbound.RetainAfterDownload.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.RetainAfterDownload') | Specifies whether the adapter will retain a file from the SFTP server after downloading it. |
| [ServerAddress](SftpAdapter.Inbound.ServerAddress.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.ServerAddress') | Specifies the server name or IP address of the secure FTP server. |
| [SshServerHostKeyFingerPrint](SftpAdapter.Inbound.SshServerHostKeyFingerPrint.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.SshServerHostKeyFingerPrint') | Specifies the fingerprint of the server used by the adapter to authenticate the server if the [AcceptAnySshServerHostKey](SftpAdapter.Inbound.AcceptAnySshServerHostKey.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.AcceptAnySshServerHostKey') property is set to `False`. If the fingerprints do not match, the connection fails. |
| [TransferMode](SftpAdapter.Inbound.TransferMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.TransferMode') | Specify the transfer mode. |
| [UserName](SftpAdapter.Inbound.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.UserName') | Specifies a username to log on to the SFTP server. |

| Methods | |
| :--- | :--- |
| [GetAddress()](SftpAdapter.Inbound.GetAddress().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.GetAddress()') | |
| [Validate()](SftpAdapter.Inbound.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound.Validate()') | |
