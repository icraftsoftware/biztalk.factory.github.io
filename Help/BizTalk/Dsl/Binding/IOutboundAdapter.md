#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## IOutboundAdapter Interface

Marker interface.

```csharp
public interface IOutboundAdapter :
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation
```

Derived  
&#8627; [Outbound](FileAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Outbound')  
&#8627; [Outbound](FtpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Outbound')  
&#8627; [Outbound](HttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound')  
&#8627; [Outbound](SBMessagingAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound')  
&#8627; [Outbound](SftpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter.Outbound')  
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
&#8627; [Outbound](WcfWebHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound')  
&#8627; [Outbound](WcfWSHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter.Outbound')

Implements [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation')