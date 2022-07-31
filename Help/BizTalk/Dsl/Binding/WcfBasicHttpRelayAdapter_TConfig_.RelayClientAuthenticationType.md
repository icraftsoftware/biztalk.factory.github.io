#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfBasicHttpRelayAdapter&lt;TConfig&gt;](WcfBasicHttpRelayAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>')

## WcfBasicHttpRelayAdapter<TConfig>.RelayClientAuthenticationType Property

Specify the option to authenticate with the Service Bus relay endpoint from where the message is received.

```csharp
public Microsoft.ServiceBus.RelayClientAuthenticationType RelayClientAuthenticationType { get; set; }
```

#### Property Value
[Microsoft.ServiceBus.RelayClientAuthenticationType](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.RelayClientAuthenticationType 'Microsoft.ServiceBus.RelayClientAuthenticationType')

### Remarks

Valid values include the following:

It defaults to [Microsoft.ServiceBus.RelayClientAuthenticationType.RelayAccessToken](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.RelayClientAuthenticationType.RelayAccessToken 'Microsoft.ServiceBus.RelayClientAuthenticationType.RelayAccessToken').