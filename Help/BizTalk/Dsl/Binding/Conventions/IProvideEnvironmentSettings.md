#### [Be.Stateless.BizTalk.Dsl.Binding.Conventions](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention](Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention')

## IProvideEnvironmentSettings Interface

Common marker interface for all overridable traits of [Platform](Platform.md 'Be.Stateless.BizTalk.Factory.Platform'), i.e. [IProvideDatabaseNames](IProvideDatabaseNames.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideDatabaseNames'),
[IProvideHostNames](IProvideHostNames.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideHostNames'), or [IProvideHostResolutionPolicy](IProvideHostResolutionPolicy.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideHostResolutionPolicy').

```csharp
public interface IProvideEnvironmentSettings
```

Derived  
&#8627; [IProvideDatabaseNames](IProvideDatabaseNames.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideDatabaseNames')  
&#8627; [IProvideHostNames](IProvideHostNames.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideHostNames')  
&#8627; [IProvideHostResolutionPolicy](IProvideHostResolutionPolicy.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideHostResolutionPolicy')  
&#8627; [Platform](Platform.md 'Be.Stateless.BizTalk.Factory.Platform')

### See Also
- [IProvideDatabaseNames](IProvideDatabaseNames.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideDatabaseNames')
- [IProvideHostNames](IProvideHostNames.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideHostNames')
- [Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportHostResolution](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportHostResolution 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportHostResolution')
- [CompositeEnvironmentSettings&lt;T,TI&gt;](CompositeEnvironmentSettings_T,TI_.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>')
- [Be.Stateless.BizTalk.Install.DeploymentContext](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.DeploymentContext 'Be.Stateless.BizTalk.Install.DeploymentContext')
- [DeploymentContext.EnvironmentSettingOverridesType](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.DeploymentContext.EnvironmentSettingOverridesType 'Be.Stateless.BizTalk.Install.DeploymentContext.EnvironmentSettingOverridesType')