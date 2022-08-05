#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWebHttpAdapter](WcfWebHttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter').[Outbound](WcfWebHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound')

## WcfWebHttpAdapter.Outbound.UseAcsAuthentication Property

Specify whether to authenticate with the Service Bus.

```csharp
public bool UseAcsAuthentication { get; set; }
```

Implements [UseAcsAuthentication](IAdapterConfigOptionalAccessControlService.UseAcsAuthentication.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOptionalAccessControlService.UseAcsAuthentication')

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks
This is required only when invoking a REST interface for Service Bus related entities.