#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter')

## FtpAdapter.Inbound Class

The FTP adapter exchanges data between an FTP server and Microsoft BizTalk Server, and allows for the integration of
vital data stored on a variety of platforms with line-of-business applications. The adapter can connect to the FTP
server via SOCKS4 or SOCKS5 proxy server.

```csharp
public class FtpAdapter.Inbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [LegacyAdapterBase](LegacyAdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.LegacyAdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.LegacyAdapterBase&lt;](LegacyAdapterBase_TValidator_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.LegacyAdapterBase<TValidator>')[Microsoft.BizTalk.Adapter.FtpAdapter.FtpAdapterManagement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.FtpAdapter.FtpAdapterManagement 'Microsoft.BizTalk.Adapter.FtpAdapter.FtpAdapterManagement')[&gt;](LegacyAdapterBase_TValidator_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.LegacyAdapterBase<TValidator>') &#129106; [FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter') &#129106; Inbound

Implements [IInboundAdapter](IInboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation')

### Remarks

The FTP adapter can transfer a large number of files from an FTP server to BizTalk Server. It can also transfer files
as part of an orchestration.

Do not configure multiple FTP receive locations to poll the same FTP URL. If multiple FTP receive locations are
polling the same URL concurrently then each receive location can receive a copy of the file, which can cause data
duplication. This behavior occurs because the FTP protocol has no provision for locking files when reading them from
the target URL.

To provide high availability for the FTP receive adapter you should configure the FTP receive adapter to run in a
clustered BizTalk Host instance. For more information about how to run an FTP receive handler in a clustered BizTalk
Host see [Considerations
            for Running Adapter Handlers within a Clustered Host](https://docs.microsoft.com/en-us/biztalk/core/considerations-for-running-adapter-handlers-within-a-clustered-host1 'https://docs.microsoft.com/en-us/biztalk/core/considerations-for-running-adapter-handlers-within-a-clustered-host1').

### See Also
- [FTP Adapter](https://docs.microsoft.com/en-us/biztalk/core/ftp-adapter 'https://docs.microsoft.com/en-us/biztalk/core/ftp-adapter')
- [Configuring the FTP Adapter](https://docs.microsoft.com/en-us/biztalk/core/configuring-the-ftp-adapter 'https://docs.microsoft.com/en-us/biztalk/core/configuring-the-ftp-adapter')
- [FTP Adapter Configuration Properties](https://docs.microsoft.com/en-us/biztalk/core/ftp-adapter-configuration-properties 'https://docs.microsoft.com/en-us/biztalk/core/ftp-adapter-configuration-properties')
- [Best practices and recommendations for the FTP Adapter](https://docs.microsoft.com/en-us/biztalk/core/best-practices-and-recommendations-for-the-ftp-adapter 'https://docs.microsoft.com/en-us/biztalk/core/best-practices-and-recommendations-for-the-ftp-adapter')
- [Known Issues with the FTP Adapter](https://docs.microsoft.com/en-us/biztalk/core/known-issues-with-the-ftp-adapter 'https://docs.microsoft.com/en-us/biztalk/core/known-issues-with-the-ftp-adapter')
- [How to Diagnose Problems with the FTP Adapter](https://docs.microsoft.com/en-us/biztalk/core/how-to-diagnose-problems-with-the-ftp-adapter 'https://docs.microsoft.com/en-us/biztalk/core/how-to-diagnose-problems-with-the-ftp-adapter')

| Constructors | |
| :--- | :--- |
| [Inbound()](FtpAdapter.Inbound.Inbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.Inbound()') | |
| [Inbound(Action&lt;Inbound&gt;)](FtpAdapter.Inbound.Inbound(Action_Inbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.Inbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound>)') | |

| Properties | |
| :--- | :--- |
| [AffiliateApplicationName](FtpAdapter.Inbound.AffiliateApplicationName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.AffiliateApplicationName') | Specify the Enterprise Single Sign-On affiliate application. |
| [AfterGet](FtpAdapter.Inbound.AfterGet.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.AfterGet') | Specify the FTP commands to run after the file `GET`. Separate commands with a semicolon (`;`). |
| [BeforeGet](FtpAdapter.Inbound.BeforeGet.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.BeforeGet') | Specify the FTP commands to run before the file `GET`. Separate commands with a semicolon (`;`). |
| [ClientCertificate](FtpAdapter.Inbound.ClientCertificate.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.ClientCertificate') | Specify the SHA1 hash of the client certificate that must be used in the Secure Sockets Layer (SSL) negotiation. |
| [DeleteAfterDownload](FtpAdapter.Inbound.DeleteAfterDownload.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.DeleteAfterDownload') | Specify whether the adapter deletes a file from the FTP server after downloading it. |
| [EnableTimestampComparison](FtpAdapter.Inbound.EnableTimestampComparison.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.EnableTimestampComparison') | Specify whether the adapter downloads a file again based on its modified timestamp. In cases when the adapter does not have delete permissions on the FTP server, the MDTM (Modification Time) command allows the adapter to know whether a file has been modified since last download. Based on the value of this property, the file is downloaded again. |
| [ErrorThreshold](FtpAdapter.Inbound.ErrorThreshold.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.ErrorThreshold') | Specify the number of errors that BizTalk Server can encounter before the location is disabled. |
| [FileMask](FtpAdapter.Inbound.FileMask.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.FileMask') | Specify the file mask filter to use when transmitting files. |
| [FirewallAddress](FtpAdapter.Inbound.FirewallAddress.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.FirewallAddress') | Specify the address of the firewall, either a DNS name or an IP address. |
| [FirewallPassword](FtpAdapter.Inbound.FirewallPassword.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.FirewallPassword') | Specify the password for the firewall. |
| [FirewallPort](FtpAdapter.Inbound.FirewallPort.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.FirewallPort') | Specify the port for the firewall. |
| [FirewallType](FtpAdapter.Inbound.FirewallType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.FirewallType') | Specify the type of firewall deployed. |
| [FirewallUserName](FtpAdapter.Inbound.FirewallUserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.FirewallUserName') | Specify the user name for the firewall. |
| [Folder](FtpAdapter.Inbound.Folder.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.Folder') | Specify the polling location on the FTP server. |
| [FtpsConnectionMode](FtpAdapter.Inbound.FtpsConnectionMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.FtpsConnectionMode') | Specify the mode of SSL connection made to the FTPS server. |
| [Log](FtpAdapter.Inbound.Log.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.Log') | Specify the location to save a copy of the log file. You use this file to diagnose error conditions when sending or receiving files through FTP. |
| [MaximumBatchSize](FtpAdapter.Inbound.MaximumBatchSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.MaximumBatchSize') | Specify the maximum number of bytes per BizTalk Server batch. |
| [MaximumFileSize](FtpAdapter.Inbound.MaximumFileSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.MaximumFileSize') | Specify the maximum file size, in megabytes, that can be downloaded. |
| [MaximumNumberOfFiles](FtpAdapter.Inbound.MaximumNumberOfFiles.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.MaximumNumberOfFiles') | Specify the maximum number of files per BizTalk Server batch. |
| [Mode](FtpAdapter.Inbound.Mode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.Mode') | Specify the mode in which the adapter connects to the FTP server. |
| [Password](FtpAdapter.Inbound.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.Password') | Specify the user password to log on to the FTP server. |
| [PollingInterval](FtpAdapter.Inbound.PollingInterval.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.PollingInterval') | Specify the interval number for polling this location. |
| [Port](FtpAdapter.Inbound.Port.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.Port') | Specify the port address for this FTP server. |
| [ReceiveTimeout](FtpAdapter.Inbound.ReceiveTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.ReceiveTimeout') | Specify the time before the receive call will abort. |
| [RedownloadInterval](FtpAdapter.Inbound.RedownloadInterval.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.RedownloadInterval') | Specify the interval after which the adapter downloads files again. |
| [Representation](FtpAdapter.Inbound.Representation.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.Representation') | Select how FTP receives the data. |
| [Server](FtpAdapter.Inbound.Server.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.Server') | Specify the server name or IP address of the FTP server. |
| [TemporaryFolder](FtpAdapter.Inbound.TemporaryFolder.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.TemporaryFolder') | Specify the location for a temporary folder. |
| [UseDataProtection](FtpAdapter.Inbound.UseDataProtection.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.UseDataProtection') | Specify if the adapter must use SSL encryption or plain text when it sends and receives data files from the FTPS server. |
| [UseNameList](FtpAdapter.Inbound.UseNameList.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.UseNameList') | Specify how the adapter lists files. To view file names instead of the system-defined file listing, set this value to `true`. |
| [UserName](FtpAdapter.Inbound.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.UserName') | Specify the user name to log on to the FTP server. |
| [UseSsl](FtpAdapter.Inbound.UseSsl.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.UseSsl') | Specify whether the FTP adapter must use SSL to communicate with the FTPS server. |
| [XmlAliasedPassiveMode](FtpAdapter.Inbound.XmlAliasedPassiveMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.XmlAliasedPassiveMode') | |
| [XmlAliasedPollingInterval](FtpAdapter.Inbound.XmlAliasedPollingInterval.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.XmlAliasedPollingInterval') | |
| [XmlAliasedPollingUnitOfMeasure](FtpAdapter.Inbound.XmlAliasedPollingUnitOfMeasure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.XmlAliasedPollingUnitOfMeasure') | |
| [XmlAliasedReceiveTimeout](FtpAdapter.Inbound.XmlAliasedReceiveTimeout.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.XmlAliasedReceiveTimeout') | |
| [XmlAliasedRedownloadInterval](FtpAdapter.Inbound.XmlAliasedRedownloadInterval.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.XmlAliasedRedownloadInterval') | |

| Methods | |
| :--- | :--- |
| [GetAddress()](FtpAdapter.Inbound.GetAddress().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound.GetAddress()') | |
