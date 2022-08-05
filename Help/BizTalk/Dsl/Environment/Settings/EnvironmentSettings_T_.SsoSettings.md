#### [Be.Stateless.BizTalk.Dsl.Environment.Settings](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Environment.Settings](Be.Stateless.BizTalk.Dsl.Environment.Settings.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings').[EnvironmentSettings&lt;T&gt;](EnvironmentSettings_T_.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>')

## EnvironmentSettings<T>.SsoSettings Property

Dictionary of environment setting properties, together with their values, that must be deployed in an SSO affiliate
application store in order to be available at runtime to the BizTalk application.

```csharp
public System.Collections.Generic.Dictionary<string,string> SsoSettings { get; }
```

Implements [SsoSettings](IProvideSsoSettings.SsoSettings.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.IProvideSsoSettings.SsoSettings')

#### Property Value
[System.Collections.Generic.Dictionary&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.Dictionary-2 'System.Collections.Generic.Dictionary`2')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.Dictionary-2 'System.Collections.Generic.Dictionary`2')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.Dictionary-2 'System.Collections.Generic.Dictionary`2')

### Remarks
Notice that the set of properties that need to be deployed in SSO is determined by the actual concrete type that
inherits from [EnvironmentSettings&lt;T&gt;](EnvironmentSettings_T_.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>'), that is to say [T](EnvironmentSettings_T_.md#Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings_T_.T 'Be.Stateless.BizTalk.Dsl.Environment.Settings.EnvironmentSettings<T>.T'), and cannot be customized
by any override type provided through [DeploymentContext.EnvironmentSettingOverridesType](DeploymentContext.EnvironmentSettingOverridesType.md 'Be.Stateless.BizTalk.Install.DeploymentContext.EnvironmentSettingOverridesType').