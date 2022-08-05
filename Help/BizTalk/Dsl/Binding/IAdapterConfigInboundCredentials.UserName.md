#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigInboundCredentials](IAdapterConfigInboundCredentials.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials')

## IAdapterConfigInboundCredentials.UserName Property

Specify the user name for this receive location to use when polling an external service to retrieve response
messages. This property is required when the [CredentialType](IAdapterConfigInboundCredentials.CredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundCredentials.CredentialType') property is set to [Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.UserAccount](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.UserAccount 'Microsoft.BizTalk.Adapter.Wcf.Config.CredentialSelection.UserAccount').

```csharp
string UserName { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
It defaults to [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty').