#### [Be.Stateless.BizTalk.Dsl.Binding.Conventions](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention](Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention').[IProvideHostResolutionPolicy](IProvideHostResolutionPolicy.md 'Be.Stateless.BizTalk.Dsl.Environment.Settings.Convention.IProvideHostResolutionPolicy')

## IProvideHostResolutionPolicy.HostResolutionPolicy Property

[Be.Stateless.BizTalk.Dsl.Binding.Convention.HostResolutionPolicy](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Binding.Convention.HostResolutionPolicy 'Be.Stateless.BizTalk.Dsl.Binding.Convention.HostResolutionPolicy')-derived policy that overrides the
            default `BizTalk.Factory`'s [HostResolutionPolicy](HostResolutionPolicy.md 'Be.Stateless.BizTalk.Factory.Convention.HostResolutionPolicy') policy in
            order to resolve the Microsoft BizTalk Server Host names for the target environment for which the [Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding 'Be.Stateless.BizTalk.Dsl.Binding.ApplicationBinding') is being XML-serialized.

```csharp
Be.Stateless.BizTalk.Dsl.Binding.Convention.HostResolutionPolicy HostResolutionPolicy { get; }
```

#### Property Value
[Be.Stateless.BizTalk.Dsl.Binding.Convention.HostResolutionPolicy](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Binding.Convention.HostResolutionPolicy 'Be.Stateless.BizTalk.Dsl.Binding.Convention.HostResolutionPolicy')

### See Also
- [Be.Stateless.BizTalk.Install.DeploymentContext](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.DeploymentContext 'Be.Stateless.BizTalk.Install.DeploymentContext')
- [Be.Stateless.BizTalk.Install.TargetEnvironment](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Install.TargetEnvironment 'Be.Stateless.BizTalk.Install.TargetEnvironment')