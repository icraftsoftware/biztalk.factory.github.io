#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')
### [Be.Stateless.BizTalk.ContextProperties](Be.Stateless.BizTalk.ContextProperties.md 'Be.Stateless.BizTalk.ContextProperties').[SftpProperties](SftpProperties.md 'Be.Stateless.BizTalk.ContextProperties.SftpProperties')

## SftpProperties.FolderPath Field

Remote SFTP folder path. Oddly enough, [FolderPath](SftpProperties.FolderPath.md 'Be.Stateless.BizTalk.ContextProperties.SftpProperties.FolderPath') is concealed in the [WCF](WCF.md 'WCF') property schema
target namespace only.

```csharp
public static readonly MessageContextProperty<FolderPath,string> FolderPath;
```

#### Field Value
[Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[FolderPath](FolderPath.md 'WCF.FolderPath')[,](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')

### Remarks

The [FolderPath](SftpProperties.FolderPath.md 'Be.Stateless.BizTalk.ContextProperties.SftpProperties.FolderPath') property is not exposed by the [SFTP](https://docs.microsoft.com/en-us/dotnet/api/SFTP 'SFTP') property schema, but at the same time,
any context override of the [FolderPath](SftpProperties.FolderPath.md 'Be.Stateless.BizTalk.ContextProperties.SftpProperties.FolderPath') value is expected to be found in the [WCF](WCF.md 'WCF') property
schema target namespace and not in its dedicated [SFTP](https://docs.microsoft.com/en-us/dotnet/api/SFTP 'SFTP') property schema target namespace.

It is essential to enable [IsDynamicSend](BtsProperties.IsDynamicSend.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties.IsDynamicSend') when setting this property at runtime.