#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigInboundCredentials](IAdapterConfigInboundCredentials.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials')

## IAdapterConfigInboundCredentials.AffiliateApplicationName Property

Specify the SSO affiliate application to return external credentials to be used when this receive location sends
solicit messages to poll an external service. The specified SSO affiliate application must have a mapping between the
Windows account under which this receive location runs and the account for the external service. This property is
required when the [CredentialType](IAdapterConfigInboundCredentials.CredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials.CredentialType') property is set to [Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.GetCredentials](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.GetCredentials 'Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.GetCredentials').

```csharp
string AffiliateApplicationName { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
It defaults to [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty').