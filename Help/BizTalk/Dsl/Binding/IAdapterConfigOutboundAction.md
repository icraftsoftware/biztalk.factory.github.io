#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## IAdapterConfigOutboundAction Interface

```csharp
public interface IAdapterConfigOutboundAction
```

Derived  
&#8627; [Outbound](WcfBasicHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter.Outbound')  
&#8627; [Outbound](WcfBasicHttpRelayAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter.Outbound')  
&#8627; [Outbound&lt;TBinding&gt;](WcfCustomAdapter.Outbound_TBinding_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Outbound<TBinding>')  
&#8627; [Outbound](WcfNetMsmqAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Outbound')  
&#8627; [Outbound](WcfNetNamedPipeAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter.Outbound')  
&#8627; [Outbound](WcfNetTcpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter.Outbound')  
&#8627; [Outbound](WcfNetTcpRelayAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpRelayAdapter.Outbound')  
&#8627; [Outbound](WcfOracleAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Outbound')  
&#8627; [Outbound](WcfSapAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound')  
&#8627; [Outbound](WcfSqlAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter.Outbound')  
&#8627; [Outbound](WcfWSHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter.Outbound')

| Properties | |
| :--- | :--- |
| [StaticAction](IAdapterConfigOutboundAction.StaticAction.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundAction.StaticAction') | Specify the SOAPAction header field for outgoing messages. This property can also be set through the message context property [WCF.Action](https://docs.microsoft.com/en-us/dotnet/api/WCF.Action 'WCF.Action') in a pipeline or orchestration. |
