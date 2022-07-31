#### [Be.Stateless.BizTalk.Dsl.Binding.Conventions](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention](Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention').[IProvideDatabaseNames](IProvideDatabaseNames.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideDatabaseNames')

## IProvideDatabaseNames.ProcessingDatabaseServer Property

Name of the SQL Server Database Server hosting the processing-related databases, e.g. `BizTalkMsgBoxDb`,
`BizTalkFactoryTransientStateDb`.

```csharp
string ProcessingDatabaseServer { get; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### See Also
- [ProcessingDatabaseInstance](IProvideDatabaseNames.ProcessingDatabaseInstance.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideDatabaseNames.ProcessingDatabaseInstance')
- [Be.Stateless.BizTalk.Install.DeploymentContext](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.DeploymentContext 'Be.Stateless.BizTalk.Install.DeploymentContext')
- [Be.Stateless.BizTalk.Install.TargetEnvironment](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.TargetEnvironment 'Be.Stateless.BizTalk.Install.TargetEnvironment')