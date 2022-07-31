#### [Be.Stateless.BizTalk.Dsl.Binding.Conventions](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention](Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention')

## IProvideDatabaseNames Interface

Elementary Microsoft BizTalk Server's Database Platform Settings that allows [Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding') to be
XML-serialized for a given target deployment environment and that provides an overriding point for [Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding') written against these settings.

```csharp
public interface IProvideDatabaseNames :
Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideEnvironmentSettings
```

Derived  
&#8627; [Platform](Platform.md 'Be.Stateless.BizTalk.Factory.Platform')

Implements [IProvideEnvironmentSettings](IProvideEnvironmentSettings.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideEnvironmentSettings')

### See Also
- [CompositeEnvironmentSettings&lt;T,TI&gt;](CompositeEnvironmentSettings_T,TI_.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>')
- [Be.Stateless.BizTalk.Install.DeploymentContext](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.DeploymentContext 'Be.Stateless.BizTalk.Install.DeploymentContext')
- [DeploymentContext.EnvironmentSettingOverridesType](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.DeploymentContext.EnvironmentSettingOverridesType 'Be.Stateless.BizTalk.Install.DeploymentContext.EnvironmentSettingOverridesType')
- [Be.Stateless.BizTalk.Install.TargetEnvironment](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.TargetEnvironment 'Be.Stateless.BizTalk.Install.TargetEnvironment')

| Properties | |
| :--- | :--- |
| [ManagementDatabaseInstance](IProvideDatabaseNames.ManagementDatabaseInstance.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideDatabaseNames.ManagementDatabaseInstance') | Name of the SQL Server Database Instance hosting the management-related databases, e.g.`BizTalkMgmtDb`, `BizTalkFactoryMgmtDb`. |
| [ManagementDatabaseServer](IProvideDatabaseNames.ManagementDatabaseServer.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideDatabaseNames.ManagementDatabaseServer') | Name of the SQL Server Database Server hosting the management-related databases, e.g.`BizTalkMgmtDb`, `BizTalkFactoryMgmtDb`. |
| [MonitoringDatabaseInstance](IProvideDatabaseNames.MonitoringDatabaseInstance.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideDatabaseNames.MonitoringDatabaseInstance') | Name of the SQL Server Database Instance hosting the monitoring-related databases, e.g. `BAMPrimaryImport`. |
| [MonitoringDatabaseServer](IProvideDatabaseNames.MonitoringDatabaseServer.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideDatabaseNames.MonitoringDatabaseServer') | Name of the SQL Server Database Server hosting the monitoring-related databases, e.g. `BAMPrimaryImport`. |
| [ProcessingDatabaseInstance](IProvideDatabaseNames.ProcessingDatabaseInstance.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideDatabaseNames.ProcessingDatabaseInstance') | Name of the SQL Server Database Instance hosting the processing-related databases, e.g. `BizTalkMsgBoxDb`, `BizTalkFactoryTransientStateDb`. |
| [ProcessingDatabaseServer](IProvideDatabaseNames.ProcessingDatabaseServer.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideDatabaseNames.ProcessingDatabaseServer') | Name of the SQL Server Database Server hosting the processing-related databases, e.g. `BizTalkMsgBoxDb`, `BizTalkFactoryTransientStateDb`. |
