#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigAccessControlService](IAdapterConfigAccessControlService.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigAccessControlService')

## IAdapterConfigAccessControlService.StsUri Property

Specify the Service Access Control Service STS URI.

```csharp
System.Uri StsUri { get; set; }
```

#### Property Value
[System.Uri](https://docs.microsoft.com/en-us/dotnet/api/System.Uri 'System.Uri')

### Remarks

Set this to `https://<namespace>-sb.accesscontrol.windows.net/`, where
<namespace> is your Service Bus namespace.

Required if [Microsoft.ServiceBus.RelayClientAuthenticationType.RelayAccessToken](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.RelayClientAuthenticationType.RelayAccessToken 'Microsoft.ServiceBus.RelayClientAuthenticationType.RelayAccessToken') is set to [Microsoft.ServiceBus.RelayClientAuthenticationType](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.RelayClientAuthenticationType 'Microsoft.ServiceBus.RelayClientAuthenticationType').