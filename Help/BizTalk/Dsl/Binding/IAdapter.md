#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## IAdapter Interface

```csharp
public interface IAdapter :
Be.Stateless.BizTalk.Dsl.ISupportValidation
```

Derived  
&#8627; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase')  
&#8627; [Inbound](FileAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound')  
&#8627; [Outbound](FileAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Outbound')  
&#8627; [Inbound](FtpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound')  
&#8627; [Outbound](FtpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound')  
&#8627; [Inbound](HttpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound')  
&#8627; [Outbound](HttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound')  
&#8627; [IInboundAdapter](IInboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter')  
&#8627; [IOutboundAdapter](IOutboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IOutboundAdapter')  
&#8627; [Inbound](Office365EmailAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound')  
&#8627; [Inbound](Pop3Adapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound')  
&#8627; [Inbound](SBMessagingAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Inbound')  
&#8627; [Outbound](SBMessagingAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound')  
&#8627; [Inbound](SftpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Inbound')  
&#8627; [Outbound](SftpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound')  
&#8627; [Inbound](WcfBasicHttpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter.Inbound')  
&#8627; [Outbound](WcfBasicHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter.Outbound')  
&#8627; [Inbound](WcfBasicHttpRelayAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter.Inbound')  
&#8627; [Outbound](WcfBasicHttpRelayAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter.Outbound')  
&#8627; [Inbound&lt;TBinding&gt;](WcfCustomAdapter.Inbound_TBinding_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>')  
&#8627; [Outbound&lt;TBinding&gt;](WcfCustomAdapter.Outbound_TBinding_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Outbound<TBinding>')  
&#8627; [Inbound&lt;TBinding&gt;](WcfCustomIsolatedAdapter.Inbound_TBinding_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>')  
&#8627; [Inbound](WcfNetMsmqAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Inbound')  
&#8627; [Outbound](WcfNetMsmqAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Outbound')  
&#8627; [Inbound](WcfNetNamedPipeAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter.Inbound')  
&#8627; [Outbound](WcfNetNamedPipeAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter.Outbound')  
&#8627; [Inbound](WcfNetTcpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter.Inbound')  
&#8627; [Outbound](WcfNetTcpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter.Outbound')  
&#8627; [Inbound](WcfNetTcpRelayAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpRelayAdapter.Inbound')  
&#8627; [Outbound](WcfNetTcpRelayAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpRelayAdapter.Outbound')  
&#8627; [Inbound](WcfOracleAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound')  
&#8627; [Outbound](WcfOracleAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Outbound')  
&#8627; [Inbound](WcfSapAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Inbound')  
&#8627; [Outbound](WcfSapAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound')  
&#8627; [Inbound](WcfSqlAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter.Inbound')  
&#8627; [Outbound](WcfSqlAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter.Outbound')  
&#8627; [Inbound](WcfWebHttpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Inbound')  
&#8627; [Outbound](WcfWebHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound')  
&#8627; [Inbound](WcfWSHttpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter.Inbound')  
&#8627; [Outbound](WcfWSHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter.Outbound')  
&#8627; [UnknownAdapter](TransportBase_T_.UnknownAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.TransportBase<T>.UnknownAdapter')

Implements [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation')

| Properties | |
| :--- | :--- |
| [Address](IAdapter.Address.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.Address') | |
| [ProtocolType](IAdapter.ProtocolType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.ProtocolType') | |
| [PublicAddress](IAdapter.PublicAddress.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.PublicAddress') | |

| Methods | |
| :--- | :--- |
| [Save(IPropertyBag)](IAdapter.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | |
