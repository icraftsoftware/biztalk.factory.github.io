#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetTcpRelayAdapter](WcfNetTcpRelayAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpRelayAdapter').[Inbound](WcfNetTcpRelayAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpRelayAdapter.Inbound')

## WcfNetTcpRelayAdapter.Inbound.RelayClientAuthenticationType Property

Specify the option to authenticate with the Service Bus relay endpoint from where the message is received.

```csharp
public Microsoft.ServiceBus.RelayClientAuthenticationType RelayClientAuthenticationType { get; set; }
```

#### Property Value
[Microsoft.ServiceBus.RelayClientAuthenticationType](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.RelayClientAuthenticationType 'Microsoft.ServiceBus.RelayClientAuthenticationType')

### Remarks

Valid values include the following:
- [Microsoft.ServiceBus.RelayClientAuthenticationType.None](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.RelayClientAuthenticationType.None 'Microsoft.ServiceBus.RelayClientAuthenticationType.None') — No authentication is required.
- [Microsoft.ServiceBus.RelayClientAuthenticationType.RelayAccessToken](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.RelayClientAuthenticationType.RelayAccessToken 'Microsoft.ServiceBus.RelayClientAuthenticationType.RelayAccessToken') — Specify this to use a security token to authorize with the Service Bus Relay endpoint.

It defaults to [Microsoft.ServiceBus.RelayClientAuthenticationType.RelayAccessToken](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.RelayClientAuthenticationType.RelayAccessToken 'Microsoft.ServiceBus.RelayClientAuthenticationType.RelayAccessToken').