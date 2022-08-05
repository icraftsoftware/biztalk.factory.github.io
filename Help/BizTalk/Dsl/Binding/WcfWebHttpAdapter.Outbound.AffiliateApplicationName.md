#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWebHttpAdapter](WcfWebHttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter').[Outbound](WcfWebHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound')

## WcfWebHttpAdapter.Outbound.AffiliateApplicationName Property

Specify the affiliate application to use for Enterprise Single Sign-On (SSO).

```csharp
public string AffiliateApplicationName { get; set; }
```

Implements [AffiliateApplicationName](IAdapterConfigOutboundCredentials.AffiliateApplicationName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundCredentials.AffiliateApplicationName')

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

You must set the credentials if you selected the [System.ServiceModel.HttpClientCredentialType.Basic](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType.Basic 'System.ServiceModel.HttpClientCredentialType.Basic') or [System.ServiceModel.HttpClientCredentialType.Digest](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType.Digest 'System.ServiceModel.HttpClientCredentialType.Digest') option for [TransportClientCredentialType](WcfWebHttpAdapter_TAddress,TConfig_.TransportClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.TransportClientCredentialType') and [UseSSO](WcfWebHttpAdapter.Outbound.UseSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound.UseSSO') is set to
`True`.

It defaults to [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty').