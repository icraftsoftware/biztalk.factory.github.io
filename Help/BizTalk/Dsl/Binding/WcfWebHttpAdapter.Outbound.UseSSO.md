#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWebHttpAdapter](WcfWebHttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter').[Outbound](WcfWebHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound')

## WcfWebHttpAdapter.Outbound.UseSSO Property

Specify whether to use Single Sign-On to retrieve client credentials for authentication with the destination
server.

```csharp
public bool UseSSO { get; set; }
```

Implements [UseSSO](IAdapterConfigSSO.UseSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO.UseSSO')

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

You must set the credentials if you selected the [System.ServiceModel.HttpClientCredentialType.Basic](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType.Basic 'System.ServiceModel.HttpClientCredentialType.Basic') or [System.ServiceModel.HttpClientCredentialType.Digest](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType.Digest 'System.ServiceModel.HttpClientCredentialType.Digest') option for [TransportClientCredentialType](WcfWebHttpAdapter_TAddress,TConfig_.TransportClientCredentialType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.TransportClientCredentialType').

It defaults to `False`.