#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter](WcfNetMsmqAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter').[Inbound](WcfNetMsmqAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound')

## WcfNetMsmqAdapter.Inbound.OrderedProcessing Property

Specify whether to process messages serially.

```csharp
public bool OrderedProcessing { get; set; }
```

Implements [OrderedProcessing](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOrdering.OrderedProcessing 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOrdering.OrderedProcessing')

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

When this property is selected, this receive location accommodates ordered message delivery when used in
conjunction with a BizTalk messaging or orchestration send port that has the `Ordered Delivery` option set to
`True`. You can select this only when the [EnableTransaction](WcfNetMsmqAdapter_TConfig_.EnableTransaction.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter<TConfig>.EnableTransaction') property
is set to `True`.

When this property is set to `True`, the WCF-NetMsmq receive location optimizes resource usage when handling
large messages by making the adapter single-threaded.

It defaults to `False`.