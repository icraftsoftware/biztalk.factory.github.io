#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SBMessagingAdapter&lt;TConfig&gt;](SBMessagingAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>')

## SBMessagingAdapter<TConfig>.Address Property

Specify the URL where the Service Bus queue is deployed.

```csharp
public System.Uri Address { get; set; }
```

Implements [Address](IAdapterConfigAddress_TAddress_.Address.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigAddress<TAddress>.Address'), [Address](IAdapter.Address.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.Address')

#### Property Value
[System.Uri](https://docs.microsoft.com/en-us/dotnet/api/System.Uri 'System.Uri')

### Remarks
The URL is generally formatted as follows: sb://<namespace>.servicebus.windows.net/<queue_name>/.