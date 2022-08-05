#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigInboundSuspendRequestMessageOnFailure](IAdapterConfigInboundSuspendRequestMessageOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundSuspendRequestMessageOnFailure')

## IAdapterConfigInboundSuspendRequestMessageOnFailure.SuspendRequestMessageOnFailure Property

Specify whether to suspend the request message that fails inbound processing due to a receive pipeline failure or a
routing failure.

```csharp
bool SuspendRequestMessageOnFailure { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks
It defaults to `True`