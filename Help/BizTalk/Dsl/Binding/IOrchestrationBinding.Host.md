#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding').[IOrchestrationBinding](IOrchestrationBinding.md 'Be.Stateless.BizTalk.Dsl.Binding.IOrchestrationBinding')

## IOrchestrationBinding.Host Property

The BizTalk Server Host Name that will host this orchestration at runtime.

```csharp
Be.Stateless.BizTalk.Dsl.Binding.Convention.HostResolutionPolicy Host { get; set; }
```

#### Property Value
[HostResolutionPolicy](HostResolutionPolicy.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.HostResolutionPolicy')

### Remarks
The [Host](IOrchestrationBinding.Host.md 'Be.Stateless.BizTalk.Dsl.Binding.IOrchestrationBinding.Host') property can either be set directly to a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') value or to a [HostResolutionPolicy](HostResolutionPolicy.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.HostResolutionPolicy')-derived object instance.