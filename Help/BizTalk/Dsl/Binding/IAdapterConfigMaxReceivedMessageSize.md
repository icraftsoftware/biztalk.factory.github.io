#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## IAdapterConfigMaxReceivedMessageSize Interface

```csharp
public interface IAdapterConfigMaxReceivedMessageSize
```

Derived  
&#8627; [WcfBasicHttpAdapter&lt;TAddress,TConfig&gt;](WcfBasicHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter<TAddress,TConfig>')  
&#8627; [WcfBasicHttpRelayAdapter&lt;TConfig&gt;](WcfBasicHttpRelayAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>')  
&#8627; [Inbound](WcfNetMsmqAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound')  
&#8627; [WcfNetNamedPipeAdapter&lt;TConfig&gt;](WcfNetNamedPipeAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter<TConfig>')  
&#8627; [WcfNetTcpAdapter&lt;TConfig&gt;](WcfNetTcpAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter<TConfig>')  
&#8627; [WcfNetTcpRelayAdapter&lt;TConfig&gt;](WcfNetTcpRelayAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpRelayAdapter<TConfig>')  
&#8627; [WcfWebHttpAdapter&lt;TAddress,TConfig&gt;](WcfWebHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>')  
&#8627; [WcfWSHttpAdapter&lt;TAddress,TConfig&gt;](WcfWSHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter<TAddress,TConfig>')

| Properties | |
| :--- | :--- |
| [MaxReceivedMessageSize](IAdapterConfigMaxReceivedMessageSize.MaxReceivedMessageSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxReceivedMessageSize.MaxReceivedMessageSize') | Specify the maximum size, in bytes, for a message (including headers) that can be received on the wire. The size of the messages is bounded by the amount of memory allocated for each message. You can use this property to limit exposure to denial of service (DoS) attacks. |
