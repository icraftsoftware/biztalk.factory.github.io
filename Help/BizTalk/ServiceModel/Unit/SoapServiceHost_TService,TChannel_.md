#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel](Be.Stateless.BizTalk.Unit.ServiceModel.md 'Be.Stateless.BizTalk.Unit.ServiceModel')

## SoapServiceHost<TService,TChannel> Class

Provides in-process self-hosting for a single endpoint of some [TService](SoapServiceHost_TService,TChannel_.md#Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost_TService,TChannel_.TService 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>.TService') service class exposing a
[TChannel](SoapServiceHost_TService,TChannel_.md#Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost_TService,TChannel_.TChannel 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>.TChannel') service contract.

```csharp
public sealed class SoapServiceHost<TService,TChannel> : Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost
    where TService : TChannel, new()
    where TChannel : class
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost_TService,TChannel_.TService'></a>

`TService`

The service class that implements the [TChannel](SoapServiceHost_TService,TChannel_.md#Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost_TService,TChannel_.TChannel 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>.TChannel') service contract.

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost_TService,TChannel_.TChannel'></a>

`TChannel`

The shape of the channel to be used to connect to the service's endpoint.

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.ServiceModel.Channels.CommunicationObject](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.CommunicationObject 'System.ServiceModel.Channels.CommunicationObject') &#129106; [System.ServiceModel.ServiceHostBase](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.ServiceHostBase 'System.ServiceModel.ServiceHostBase') &#129106; [System.ServiceModel.ServiceHost](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.ServiceHost 'System.ServiceModel.ServiceHost') &#129106; [SoapServiceHost](SoapServiceHost.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost') &#129106; SoapServiceHost<TService,TChannel>

### Remarks

The only purpose of the [SoapServiceHost&lt;TService,TChannel&gt;](SoapServiceHost_TService,TChannel_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>') is to support WCF service hosting for the sake
of unit testing. Even though one can always mock a service contract, sometimes nothing compares to the real thing when
one has to do WCF plumbing.

Notice that [SoapServiceHost&lt;TService,TChannel&gt;](SoapServiceHost_TService,TChannel_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>') will systematically try to register a metadata exchange
endpoint, in accordance to the address' scheme, at the relative `mex` address. [SoapServiceHost&lt;TService,TChannel&gt;](SoapServiceHost_TService,TChannel_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>') might consequently fail to start if there is no [System.ServiceModel.Channels.Binding](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Binding 'System.ServiceModel.Channels.Binding') that
supports the exchange of metadata over the [Endpoint](SoapServiceHost_TService,TChannel_.Endpoint.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>.Endpoint')'s address scheme; see also [System.ServiceModel.Description.MetadataExchangeBindings](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Description.MetadataExchangeBindings 'System.ServiceModel.Description.MetadataExchangeBindings').

### See Also
- [System.ServiceModel.Description.MetadataExchangeBindings](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Description.MetadataExchangeBindings 'System.ServiceModel.Description.MetadataExchangeBindings')

| Properties | |
| :--- | :--- |
| [ChannelType](SoapServiceHost_TService,TChannel_.ChannelType.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>.ChannelType') | |
| [Endpoint](SoapServiceHost_TService,TChannel_.Endpoint.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>.Endpoint') | |
| [ServiceType](SoapServiceHost_TService,TChannel_.ServiceType.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>.ServiceType') | |

| Methods | |
| :--- | :--- |
| [Initialize(Uri)](SoapServiceHost_TService,TChannel_.Initialize(Uri).md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>.Initialize(System.Uri)') | |
