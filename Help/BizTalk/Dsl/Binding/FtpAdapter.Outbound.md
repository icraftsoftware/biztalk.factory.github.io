#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter')

## FtpAdapter.Outbound Class

The FTP adapter exchanges data between an FTP server and Microsoft BizTalk Server, and allows for the integration of
vital data stored on a variety of platforms with line-of-business applications. The adapter can connect to the FTP
server via SOCKS4 or SOCKS5 proxy server.

```csharp
public class FtpAdapter.Outbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IOutboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [LegacyAdapterBase](LegacyAdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.LegacyAdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.LegacyAdapterBase&lt;](LegacyAdapterBase_TValidator_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.LegacyAdapterBase<TValidator>')[Microsoft.BizTalk.Adapter.FtpAdapter.FtpAdapterManagement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.FtpAdapter.FtpAdapterManagement 'Microsoft.BizTalk.Adapter.FtpAdapter.FtpAdapterManagement')[&gt;](LegacyAdapterBase_TValidator_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.LegacyAdapterBase<TValidator>') &#129106; [FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter') &#129106; Outbound

Implements [IOutboundAdapter](IOutboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IOutboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation')

### Remarks
The FTP adapter can transfer a large number of files from an FTP server to BizTalk Server. It can also transfer files
as part of an orchestration.

### See Also
- [FTP Adapter](https://docs.microsoft.com/en-us/biztalk/core/ftp-adapter 'https://docs.microsoft.com/en-us/biztalk/core/ftp-adapter')
- [Configuring the FTP Adapter](https://docs.microsoft.com/en-us/biztalk/core/configuring-the-ftp-adapter 'https://docs.microsoft.com/en-us/biztalk/core/configuring-the-ftp-adapter')
- [Best practices and recommendations for the FTP Adapter](https://docs.microsoft.com/en-us/biztalk/core/best-practices-and-recommendations-for-the-ftp-adapter 'https://docs.microsoft.com/en-us/biztalk/core/best-practices-and-recommendations-for-the-ftp-adapter')

| Constructors | |
| :--- | :--- |
| [Outbound()](FtpAdapter.Outbound.Outbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.Outbound()') | |
| [Outbound(Action&lt;Outbound&gt;)](FtpAdapter.Outbound.Outbound(Action_Outbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.Outbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound>)') | |

| Properties | |
| :--- | :--- |
| [AffiliateApplicationName](FtpAdapter.Outbound.AffiliateApplicationName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.AffiliateApplicationName') | Specify the Enterprise Single Sign-On affiliate application. |
| [AfterPut](FtpAdapter.Outbound.AfterPut.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.AfterPut') | Specify the FTP commands to run after the file `PUT`. Separate commands with a semicolon (`;`). |
| [AllocateStorage](FtpAdapter.Outbound.AllocateStorage.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.AllocateStorage') | Specify whether to allocate storage space for legacy host systems. This option is provided for backward compatibility. |
| [AppendIfExists](FtpAdapter.Outbound.AppendIfExists.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.AppendIfExists') | Specify to append data to file if it exists. |
| [BeforePut](FtpAdapter.Outbound.BeforePut.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.BeforePut') | Specify the FTP commands to run before the file `PUT`. Separate commands with a semicolon (`;`). |
| [ClientCertificate](FtpAdapter.Outbound.ClientCertificate.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.ClientCertificate') | Specify the SHA1 hash of the client certificate that must be used in the Secure Sockets Layer (SSL) negotiation. |
| [ConnectionLimit](FtpAdapter.Outbound.ConnectionLimit.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.ConnectionLimit') | Specify the maximum number of concurrent FTP connections that can be opened to the server. A value of 0 means no limit. |
| [FirewallAddress](FtpAdapter.Outbound.FirewallAddress.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.FirewallAddress') | Specify the address of the firewall, either a DNS name or an IP address. |
| [FirewallPassword](FtpAdapter.Outbound.FirewallPassword.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.FirewallPassword') | Specify the password for the firewall. |
| [FirewallPort](FtpAdapter.Outbound.FirewallPort.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.FirewallPort') | Specify the port for the firewall. |
| [FirewallType](FtpAdapter.Outbound.FirewallType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.FirewallType') | Specify the type of firewall deployed. |
| [FirewallUserName](FtpAdapter.Outbound.FirewallUserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.FirewallUserName') | Specify the user name for the firewall. |
| [Folder](FtpAdapter.Outbound.Folder.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.Folder') | Specify the location to move the files to on the FTP server. |
| [FtpsConnectionMode](FtpAdapter.Outbound.FtpsConnectionMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.FtpsConnectionMode') | Specify the mode of SSL connection made to the FTPS server. |
| [Log](FtpAdapter.Outbound.Log.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.Log') | Specify the location to save a copy of the log file. Use this file to diagnose error conditions when sending or receiving files through FTP adapter. |
| [Mode](FtpAdapter.Outbound.Mode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.Mode') | Specify the mode in which the adapter connects to the FTP server. |
| [Password](FtpAdapter.Outbound.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.Password') | Specify the user password to log on to the FTP server. |
| [Port](FtpAdapter.Outbound.Port.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.Port') | Specify the port address for this FTP server. |
| [Representation](FtpAdapter.Outbound.Representation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.Representation') | Select how FTP receives the data. |
| [Server](FtpAdapter.Outbound.Server.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.Server') | Specify the server name or IP address of the FTP server. |
| [TargetFileName](FtpAdapter.Outbound.TargetFileName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.TargetFileName') | Specify an alternative name for the file. Retaining the default name guarantees unique message names for each message sent. |
| [TemporaryFolder](FtpAdapter.Outbound.TemporaryFolder.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.TemporaryFolder') | Specify the location for a temporary folder. |
| [UseDataProtection](FtpAdapter.Outbound.UseDataProtection.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.UseDataProtection') | Specify if the adapter must use SSL encryption or plain text when it sends and receives data files from the FTPS server. |
| [UserName](FtpAdapter.Outbound.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.UserName') | Specify the user name to log on to the FTP server. |
| [UseSsl](FtpAdapter.Outbound.UseSsl.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.UseSsl') | Specify whether the FTP adapter must use SSL to communicate with the FTPS server. |
| [XmlAliasedPassiveMode](FtpAdapter.Outbound.XmlAliasedPassiveMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.XmlAliasedPassiveMode') | |

| Methods | |
| :--- | :--- |
| [GetAddress()](FtpAdapter.Outbound.GetAddress().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound.GetAddress()') | |
