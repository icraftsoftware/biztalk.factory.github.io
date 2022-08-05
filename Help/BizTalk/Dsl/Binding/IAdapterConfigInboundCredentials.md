#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## IAdapterConfigInboundCredentials Interface

```csharp
public interface IAdapterConfigInboundCredentials
```

Derived  
&#8627; [Inbound&lt;TBinding&gt;](WcfCustomAdapter.Inbound_TBinding_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomAdapter.Inbound<TBinding>')  
&#8627; [Inbound&lt;TBinding&gt;](WcfCustomIsolatedAdapter.Inbound_TBinding_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfCustomIsolatedAdapter.Inbound<TBinding>')  
&#8627; [Inbound](WcfOracleAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter.Inbound')  
&#8627; [Inbound](WcfSapAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Inbound')  
&#8627; [Inbound](WcfSqlAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter.Inbound')

| Properties | |
| :--- | :--- |
| [AffiliateApplicationName](IAdapterConfigInboundCredentials.AffiliateApplicationName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials.AffiliateApplicationName') | Specify the SSO affiliate application to return external credentials to be used when this receive location sends solicit messages to poll an external service. The specified SSO affiliate application must have a mapping between the Windows account under which this receive location runs and the account for the external service. This property is required when the [CredentialType](IAdapterConfigInboundCredentials.CredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials.CredentialType') property is set to [Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.GetCredentials](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.GetCredentials 'Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.GetCredentials'). |
| [CredentialType](IAdapterConfigInboundCredentials.CredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials.CredentialType') | Specify the type of credentials for this receive location to use when polling an external service. |
| [Password](IAdapterConfigInboundCredentials.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials.Password') | Specify the password for this receive location to use when polling an external service to retrieve response messages. This property is required when the [CredentialType](IAdapterConfigInboundCredentials.CredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials.CredentialType') property is set to [Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.UserAccount](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.UserAccount 'Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.UserAccount'). |
| [UserName](IAdapterConfigInboundCredentials.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials.UserName') | Specify the user name for this receive location to use when polling an external service to retrieve response messages. This property is required when the [CredentialType](IAdapterConfigInboundCredentials.CredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials.CredentialType') property is set to [Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.UserAccount](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.UserAccount 'Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.UserAccount'). |
