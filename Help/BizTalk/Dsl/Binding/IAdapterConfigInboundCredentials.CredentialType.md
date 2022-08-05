#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigInboundCredentials](IAdapterConfigInboundCredentials.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials')

## IAdapterConfigInboundCredentials.CredentialType Property

Specify the type of credentials for this receive location to use when polling an external service.

```csharp
Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection CredentialType { get; set; }
```

#### Property Value
[Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection 'Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection')

### Remarks

- [Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.None](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.None 'Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.None') — Do not use any credentials when this receive location sends solicit
              messages to poll an external service, or this receive location does not need to poll any external service.
- [Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.IssueTicket](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.IssueTicket 'Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.IssueTicket') — Use Enterprise Single Sign-On (SSO) to retrieve client
              credentials to issue an SSO ticket. This option requires using the security mode that allows this receive location to
              impersonate the user account to issue an SSO ticket.
- [Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.UserAccount](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.UserAccount 'Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.UserAccount') — Use the credentials specified in the [UserName](IAdapterConfigInboundCredentials.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials.UserName') and
              [Password](IAdapterConfigInboundCredentials.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials.Password') properties when this receive location sends solicit messages to poll an external service.
- [Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.GetCredentials](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.GetCredentials 'Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.GetCredentials') — Use the SSO affiliate application specified in the [AffiliateApplicationName](IAdapterConfigInboundCredentials.AffiliateApplicationName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials.AffiliateApplicationName') property when this receive location sends solicit messages to poll an external
              service.

It defaults to [Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.None](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.None 'Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.None').