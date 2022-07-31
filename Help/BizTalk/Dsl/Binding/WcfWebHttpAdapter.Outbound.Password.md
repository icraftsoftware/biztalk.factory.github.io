#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWebHttpAdapter](WcfWebHttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter').[Outbound](WcfWebHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound')

## WcfWebHttpAdapter.Outbound.Password Property

Specify the password to use for authentication with the destination server when the [UseSSO](WcfWebHttpAdapter.Outbound.UseSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound.UseSSO') property
is set to `False`.

```csharp
public string Password { get; set; }
```

Implements [Password](IAdapterConfigOutboundCredentials.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundCredentials.Password')

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

You must set the credentials if you selected the [System.ServiceModel.HttpClientCredentialType.Basic](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType.Basic 'System.ServiceModel.HttpClientCredentialType.Basic') or [System.ServiceModel.HttpClientCredentialType.Digest](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType.Digest 'System.ServiceModel.HttpClientCredentialType.Digest') option for [TransportClientCredentialType](WcfWebHttpAdapter_TAddress,TConfig_.TransportClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.TransportClientCredentialType') and [UseSSO](WcfWebHttpAdapter.Outbound.UseSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound.UseSSO') is set to
`False`.

It defaults to [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty').