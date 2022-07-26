#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.ContextProperties](Be.Stateless.BizTalk.ContextProperties.md 'Be.Stateless.BizTalk.ContextProperties')

## SftpProperties Class

Allow usage of all [SFTP](https://docs.microsoft.com/en-us/dotnet/api/SFTP 'SFTP') properties, including [FolderPath](SftpProperties.FolderPath.md 'Be.Stateless.BizTalk.ContextProperties.SftpProperties.FolderPath'), through the [WCF](WCF.md 'WCF')
property schema target namespace, which has runtime precedence over the dedicated [SFTP](https://docs.microsoft.com/en-us/dotnet/api/SFTP 'SFTP') property schema
target namespace.

```csharp
public abstract class SftpProperties
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; SftpProperties

### Remarks

Notice that [FolderPath](SftpProperties.FolderPath.md 'Be.Stateless.BizTalk.ContextProperties.SftpProperties.FolderPath') is not declared by its dedicated [SFTP](https://docs.microsoft.com/en-us/dotnet/api/SFTP 'SFTP') property schema and can
therefore only be used through the [WCF](WCF.md 'WCF') property schema target namespace.

It is essential to enable [IsDynamicSend](BtsProperties.IsDynamicSend.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.IsDynamicSend') when setting the [FolderPath](SftpProperties.FolderPath.md 'Be.Stateless.BizTalk.ContextProperties.SftpProperties.FolderPath') property
at runtime.

| Fields | |
| :--- | :--- |
| [FolderPath](SftpProperties.FolderPath.md 'Be.Stateless.BizTalk.ContextProperties.SftpProperties.FolderPath') | Remote SFTP folder path. Oddly enough, [FolderPath](SftpProperties.FolderPath.md 'Be.Stateless.BizTalk.ContextProperties.SftpProperties.FolderPath') is concealed in the [WCF](WCF.md 'WCF') property schema target namespace only. |
| [TargetFileName](SftpProperties.TargetFileName.md 'Be.Stateless.BizTalk.ContextProperties.SftpProperties.TargetFileName') | Remote SFTP file name. |
