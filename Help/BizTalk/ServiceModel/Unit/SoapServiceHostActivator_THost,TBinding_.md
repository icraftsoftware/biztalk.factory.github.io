#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel](Be.Stateless.BizTalk.Unit.ServiceModel.md 'Be.Stateless.BizTalk.Unit.ServiceModel')

## SoapServiceHostActivator<THost,TBinding> Class

Starts the [SoapServiceHost&lt;TService,TChannel&gt;](SoapServiceHost_TService,TChannel_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>')-derived in-process [System.ServiceModel.ServiceHost](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.ServiceHost 'System.ServiceModel.ServiceHost') that hosts a
WCF service endpoint for the purpose of unit testing a WCF service or its their contracts.

```csharp
public abstract class SoapServiceHostActivator<THost,TBinding> :
Be.Stateless.BizTalk.Unit.ServiceModel.ISoapServiceHost,
System.IDisposable
    where THost : Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost, new()
    where TBinding : System.ServiceModel.Channels.Binding, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator_THost,TBinding_.THost'></a>

`THost`

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator_THost,TBinding_.TBinding'></a>

`TBinding`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; SoapServiceHostActivator<THost,TBinding>

Derived  
&#8627; [SoapStubHostActivator](SoapStubHostActivator.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStubHostActivator')

Implements [ISoapServiceHost](ISoapServiceHost.md 'Be.Stateless.BizTalk.Unit.ServiceModel.ISoapServiceHost'), [System.IDisposable](https://docs.microsoft.com/en-us/dotnet/api/System.IDisposable 'System.IDisposable')

### Remarks
[SoapServiceHostActivator&lt;THost,TBinding&gt;](SoapServiceHostActivator_THost,TBinding_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator<THost,TBinding>') ensures that the [SoapServiceHost&lt;TService,TChannel&gt;](SoapServiceHost_TService,TChannel_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>')-derived in-process [System.ServiceModel.ServiceHost](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.ServiceHost 'System.ServiceModel.ServiceHost') is started so that its hosted
            WCF service endpoint is listening and started before any unit test depending on it runs.

### See Also
- [SoapServiceHost&lt;TService,TChannel&gt;](SoapServiceHost_TService,TChannel_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>')

| Constructors | |
| :--- | :--- |
| [SoapServiceHostActivator(Uri)](SoapServiceHostActivator_THost,TBinding_.SoapServiceHostActivator(Uri).md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator<THost,TBinding>.SoapServiceHostActivator(System.Uri)') | |

| Fields | |
| :--- | :--- |
| [Binding](SoapServiceHostActivator_THost,TBinding_.Binding.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator<THost,TBinding>.Binding') | |

| Properties | |
| :--- | :--- |
| [Host](SoapServiceHostActivator_THost,TBinding_.Host.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator<THost,TBinding>.Host') | |

| Methods | |
| :--- | :--- |
| [Dispose()](SoapServiceHostActivator_THost,TBinding_.Dispose().md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator<THost,TBinding>.Dispose()') | |
