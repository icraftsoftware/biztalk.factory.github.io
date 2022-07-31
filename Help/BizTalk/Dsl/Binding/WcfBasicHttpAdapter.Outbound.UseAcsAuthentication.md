#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfBasicHttpAdapter](WcfBasicHttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter').[Outbound](WcfBasicHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter.Outbound')

## WcfBasicHttpAdapter.Outbound.UseAcsAuthentication Property

Access Control Service (ACS) must be configured to issue token in Simple Web Token (SWT) format using a service
identity symmetric key. The SWT token will be sent in the HTTP Authorization header.

```csharp
public bool UseAcsAuthentication { get; set; }
```

Implements [UseAcsAuthentication](IAdapterConfigOptionalAccessControlService.UseAcsAuthentication.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOptionalAccessControlService.UseAcsAuthentication')

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')