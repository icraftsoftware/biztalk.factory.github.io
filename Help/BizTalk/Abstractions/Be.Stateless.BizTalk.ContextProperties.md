#### [Be.Stateless.BizTalk.Abstractions](README.md 'README')

## Be.Stateless.BizTalk.ContextProperties Namespace

| Classes | |
| :--- | :--- |
| [BizTalkFactoryProperties](BizTalkFactoryProperties.md 'Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties') | |
| [BtsProperties](BtsProperties.md 'Be.Stateless.BizTalk.ContextProperties.BtsProperties') | System properties are mostly used internally by BizTalk Messaging Engine and its components. In general, changing the values set by the engine for those properties is not recommended, because it may affect the execution logic of the engine. However, there are a large number of properties that you can change. |
| [EdiProperties](EdiProperties.md 'Be.Stateless.BizTalk.ContextProperties.EdiProperties') | |
| [ErrorReportProperties](ErrorReportProperties.md 'Be.Stateless.BizTalk.ContextProperties.ErrorReportProperties') | The properties that are promoted to the context of an error message. |
| [FileProperties](FileProperties.md 'Be.Stateless.BizTalk.ContextProperties.FileProperties') | |
| [HttpProperties](HttpProperties.md 'Be.Stateless.BizTalk.ContextProperties.HttpProperties') | |
| [MessageContextProperty&lt;T,TR&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>') | Strong-typing wrapper for any [Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase 'Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase')-derived property. |
| [OverridableEdiProperties](OverridableEdiProperties.md 'Be.Stateless.BizTalk.ContextProperties.OverridableEdiProperties') | |
| [Pop3Properties](Pop3Properties.md 'Be.Stateless.BizTalk.ContextProperties.Pop3Properties') | |
| [SapProperties](SapProperties.md 'Be.Stateless.BizTalk.ContextProperties.SapProperties') | |
| [SBMessagingProperties](SBMessagingProperties.md 'Be.Stateless.BizTalk.ContextProperties.SBMessagingProperties') | |
| [SftpProperties](SftpProperties.md 'Be.Stateless.BizTalk.ContextProperties.SftpProperties') | Allow usage of all [SFTP](https://docs.microsoft.com/en-us/dotnet/api/SFTP 'SFTP') properties, including [FolderPath](SftpProperties.FolderPath.md 'Be.Stateless.BizTalk.ContextProperties.SftpProperties.FolderPath'), through the [WCF](WCF.md 'WCF') property schema target namespace, which has runtime precedence over the dedicated [SFTP](https://docs.microsoft.com/en-us/dotnet/api/SFTP 'SFTP') property schema target namespace. |
| [WcfProperties](WcfProperties.md 'Be.Stateless.BizTalk.ContextProperties.WcfProperties') | |
| [XmlNormProperties](XmlNormProperties.md 'Be.Stateless.BizTalk.ContextProperties.XmlNormProperties') | |

| Interfaces | |
| :--- | :--- |
| [IMessageContextProperty](IMessageContextProperty.md 'Be.Stateless.BizTalk.ContextProperties.IMessageContextProperty') | Interface contract of the strong-typing wrapper for any [MessageContextProperty&lt;T,TR&gt;](MessageContextProperty_T,TR_.md 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>')-derived property, [Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase 'Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase'). |
