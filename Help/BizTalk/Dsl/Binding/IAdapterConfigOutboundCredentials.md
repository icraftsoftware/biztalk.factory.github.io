#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## IAdapterConfigOutboundCredentials Interface

```csharp
public interface IAdapterConfigOutboundCredentials :
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO
```

Derived  
&#8627; [Outbound](HttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound')  
&#8627; [Outbound](WcfBasicHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter.Outbound')  
&#8627; [Outbound&lt;TBinding&gt;](WcfCustomAdapter.Outbound_TBinding_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Outbound<TBinding>')  
&#8627; [Outbound](WcfNetMsmqAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetMsmqAdapter.Outbound')  
&#8627; [Outbound](WcfNetTcpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetTcpAdapter.Outbound')  
&#8627; [Outbound](WcfOracleAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Outbound')  
&#8627; [Outbound](WcfSapAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound')  
&#8627; [Outbound](WcfSqlAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter.Outbound')  
&#8627; [Outbound](WcfWebHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound')  
&#8627; [Outbound](WcfWSHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter.Outbound')

Implements [IAdapterConfigSSO](IAdapterConfigSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO')

| Properties | |
| :--- | :--- |
| [AffiliateApplicationName](IAdapterConfigOutboundCredentials.AffiliateApplicationName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundCredentials.AffiliateApplicationName') | Specify the affiliate application to use for Enterprise Single Sign-On (SSO). |
| [Password](IAdapterConfigOutboundCredentials.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundCredentials.Password') | Specify the password to use for authentication with the destination server when the [UseSSO](IAdapterConfigSSO.UseSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO.UseSSO') property is set to `False`. |
| [UserName](IAdapterConfigOutboundCredentials.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundCredentials.UserName') | Specify the user name to use for authentication with the destination server when the [UseSSO](IAdapterConfigSSO.UseSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO.UseSSO') property is set to `False`. |
