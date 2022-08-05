#### [Be.Stateless.BizTalk.Dsl.Binding.Conventions](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention](Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention')

## IProvideHostNames Interface

Elementary Microsoft BizTalk Server's Host Platform Settings that allows [Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding') to be
XML-serialized for a given target deployment environment and that provides an overriding point for [Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding') written against these settings.

```csharp
public interface IProvideHostNames :
Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideEnvironmentSettings
```

Derived  
&#8627; [Platform](Platform.md 'Be.Stateless.BizTalk.Factory.Platform')

Implements [IProvideEnvironmentSettings](IProvideEnvironmentSettings.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideEnvironmentSettings')

### Remarks
The [DeploymentContext.EnvironmentSettingOverridesType](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.DeploymentContext.EnvironmentSettingOverridesType 'Be.Stateless.BizTalk.Install.DeploymentContext.EnvironmentSettingOverridesType')
overriding [IProvideHostNames](IProvideHostNames.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideHostNames') cannot override [Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportHostResolution](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportHostResolution 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportHostResolution') at the same time.

### See Also
- [CompositeEnvironmentSettings&lt;T,TI&gt;](CompositeEnvironmentSettings_T,TI_.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.CompositeEnvironmentSettings<T,TI>')
- [Be.Stateless.BizTalk.Install.DeploymentContext](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.DeploymentContext 'Be.Stateless.BizTalk.Install.DeploymentContext')
- [DeploymentContext.EnvironmentSettingOverridesType](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.DeploymentContext.EnvironmentSettingOverridesType 'Be.Stateless.BizTalk.Install.DeploymentContext.EnvironmentSettingOverridesType')
- [Be.Stateless.BizTalk.Install.TargetEnvironment](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.TargetEnvironment 'Be.Stateless.BizTalk.Install.TargetEnvironment')
- [Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportHostResolution](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportHostResolution 'Be.Stateless.BizTalk.Dsl.Binding.Convention.ISupportHostResolution')

| Properties | |
| :--- | :--- |
| [IsolatedHost](IProvideHostNames.IsolatedHost.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideHostNames.IsolatedHost') | Name of the Microsoft BizTalk Server isolated host in the target deployment environment. |
| [ProcessingHost](IProvideHostNames.ProcessingHost.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideHostNames.ProcessingHost') | Name of the Microsoft BizTalk Server host that will host orchestrations in the target deployment environment. |
| [ReceivingHost](IProvideHostNames.ReceivingHost.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideHostNames.ReceivingHost') | Name of the Microsoft BizTalk Server host that will host receive locations in the target deployment environment. |
| [TransmittingHost](IProvideHostNames.TransmittingHost.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideHostNames.TransmittingHost') | Name of the Microsoft BizTalk Server host that will host send ports in the target deployment environment. |
