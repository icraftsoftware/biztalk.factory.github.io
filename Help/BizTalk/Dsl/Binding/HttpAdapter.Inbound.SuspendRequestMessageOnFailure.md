#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter').[Inbound](HttpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound')

## HttpAdapter.Inbound.SuspendRequestMessageOnFailure Property

Indicate whether or not to suspend HTTP requests that fail inbound processing.

```csharp
public bool SuspendRequestMessageOnFailure { get; set; }
```

Implements [SuspendRequestMessageOnFailure](IAdapterConfigInboundSuspendRequestMessageOnFailure.SuspendRequestMessageOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundSuspendRequestMessageOnFailure.SuspendRequestMessageOnFailure')

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

A value of `False` indicates to discard the failed request and send an error status code (401 or 500) to the
client.

A value of `True` indicates to suspend the failed request and send an "Accepted" status code (202) to the
client for one-way receive ports or an "Error" status code (500) to the client for two-way receive ports.

It defaults to `True`.