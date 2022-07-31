#### [Be.Stateless.BizTalk.Dsl.Binding.Conventions](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention](Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention').[IProvideDatabaseNames](IProvideDatabaseNames.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideDatabaseNames')

## IProvideDatabaseNames.ProcessingDatabaseInstance Property

Name of the SQL Server Database Instance hosting the processing-related databases, e.g. `BizTalkMsgBoxDb`,
`BizTalkFactoryTransientStateDb`.

```csharp
string ProcessingDatabaseInstance { get; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### See Also
- [ProcessingDatabaseServer](IProvideDatabaseNames.ProcessingDatabaseServer.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideDatabaseNames.ProcessingDatabaseServer')
- [Be.Stateless.BizTalk.Install.DeploymentContext](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.DeploymentContext 'Be.Stateless.BizTalk.Install.DeploymentContext')
- [Be.Stateless.BizTalk.Install.TargetEnvironment](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.TargetEnvironment 'Be.Stateless.BizTalk.Install.TargetEnvironment')