#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfCustomAdapter](WcfCustomAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter').[Inbound&lt;TBinding&gt;](WcfCustomAdapter.Inbound_TBinding_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>')

## WcfCustomAdapter.Inbound<TBinding>.OrderedProcessing Property

Specify whether to preserve message order when processing messages received over the NetMsmq binding.

```csharp
public bool OrderedProcessing { get; set; }
```

Implements [OrderedProcessing](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOrdering.OrderedProcessing 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOrdering.OrderedProcessing')

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks
It defaults to `False`