#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetMsmqAdapter](WcfNetMsmqAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter').[Outbound](WcfNetMsmqAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Outbound')

## WcfNetMsmqAdapter.Outbound.UseSourceJournal Property

Specify whether copies of messages processed by this send port should be stored in the source journal queue.

```csharp
public bool UseSourceJournal { get; set; }
```

Implements [UseSourceJournal](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqBinding.UseSourceJournal 'Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigNetMsmqBinding.UseSourceJournal')

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks
It defaults to `False`.