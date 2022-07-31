#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigInboundDisableLocationOnFailure](IAdapterConfigInboundDisableLocationOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundDisableLocationOnFailure')

## IAdapterConfigInboundDisableLocationOnFailure.DisableLocationOnFailure Property

Specify whether to disable the receive location that fails inbound processing due to a receive pipeline failure or a
routing failure.

```csharp
bool DisableLocationOnFailure { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks
It defaults to `False`