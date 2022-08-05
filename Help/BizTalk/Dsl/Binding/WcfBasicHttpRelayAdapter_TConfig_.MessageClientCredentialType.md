#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfBasicHttpRelayAdapter&lt;TConfig&gt;](WcfBasicHttpRelayAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>')

## WcfBasicHttpRelayAdapter<TConfig>.MessageClientCredentialType Property

Specify the message-level security options only if you set the Security mode above to Message or
TransportWithMessageCredential.

```csharp
public System.ServiceModel.BasicHttpMessageCredentialType MessageClientCredentialType { get; set; }
```

Implements [MessageClientCredentialType](IAdapterConfigMessageSecurity_T_.MessageClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageSecurity<T>.MessageClientCredentialType')

#### Property Value
[System.ServiceModel.BasicHttpMessageCredentialType](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpMessageCredentialType 'System.ServiceModel.BasicHttpMessageCredentialType')

### Remarks

Valid values include the following:
- UserName — Enables this receive location to require that clients be authenticated using the UserName credential. You must create
  the domain or local user accounts corresponding to the client credentials.
- Certificate — Clients are authenticated to this receive location using the client certificate. The CA certificate chain for the
  client X.509 certificates must be installed in the Trusted Root Certification Authorities certificate store of this
  computer so that the clients can be authenticated to this receive

It defaults to [System.ServiceModel.BasicHttpMessageCredentialType.UserName](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpMessageCredentialType.UserName 'System.ServiceModel.BasicHttpMessageCredentialType.UserName').