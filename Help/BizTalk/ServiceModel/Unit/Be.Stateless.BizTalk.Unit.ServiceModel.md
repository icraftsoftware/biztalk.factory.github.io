#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')

## Be.Stateless.BizTalk.Unit.ServiceModel Namespace

| Classes | |
| :--- | :--- |
| [RestClient](RestClient.md 'Be.Stateless.BizTalk.Unit.ServiceModel.RestClient') | |
| [SoapClient](SoapClient.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapClient') | |
| [SoapClient&lt;TChannel&gt;](SoapClient_TChannel_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapClient<TChannel>') | |
| [SoapServiceHost](SoapServiceHost.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost') | |
| [SoapServiceHost&lt;TService,TChannel&gt;](SoapServiceHost_TService,TChannel_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>') | Provides in-process self-hosting for a single endpoint of some [TService](SoapServiceHost_TService,TChannel_.md#Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost_TService,TChannel_.TService 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>.TService') service class exposing a [TChannel](SoapServiceHost_TService,TChannel_.md#Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost_TService,TChannel_.TChannel 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>.TChannel') service contract. |
| [SoapServiceHostActivator&lt;THost,TBinding&gt;](SoapServiceHostActivator_THost,TBinding_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator<THost,TBinding>') | Starts the [SoapServiceHost&lt;TService,TChannel&gt;](SoapServiceHost_TService,TChannel_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost<TService,TChannel>')-derived in-process [System.ServiceModel.ServiceHost](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.ServiceHost 'System.ServiceModel.ServiceHost') that hosts a WCF service endpoint for the purpose of unit testing a WCF service or its their contracts. |

| Interfaces | |
| :--- | :--- |
| [ISoapServiceHost](ISoapServiceHost.md 'Be.Stateless.BizTalk.Unit.ServiceModel.ISoapServiceHost') | |
