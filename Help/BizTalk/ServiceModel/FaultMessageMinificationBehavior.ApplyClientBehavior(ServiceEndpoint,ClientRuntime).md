#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Description](Be.Stateless.BizTalk.ServiceModel.Description.md 'Be.Stateless.BizTalk.ServiceModel.Description').[FaultMessageMinificationBehavior](FaultMessageMinificationBehavior.md 'Be.Stateless.BizTalk.ServiceModel.Description.FaultMessageMinificationBehavior')

## FaultMessageMinificationBehavior.ApplyClientBehavior(ServiceEndpoint, ClientRuntime) Method

Implements a modification or extension of the client across an endpoint.

```csharp
public void ApplyClientBehavior(System.ServiceModel.Description.ServiceEndpoint endpoint, System.ServiceModel.Dispatcher.ClientRuntime clientRuntime);
```
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Description.FaultMessageMinificationBehavior.ApplyClientBehavior(System.ServiceModel.Description.ServiceEndpoint,System.ServiceModel.Dispatcher.ClientRuntime).endpoint'></a>

`endpoint` [System.ServiceModel.Description.ServiceEndpoint](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Description.ServiceEndpoint 'System.ServiceModel.Description.ServiceEndpoint')

The endpoint that is to be customized.

<a name='Be.Stateless.BizTalk.ServiceModel.Description.FaultMessageMinificationBehavior.ApplyClientBehavior(System.ServiceModel.Description.ServiceEndpoint,System.ServiceModel.Dispatcher.ClientRuntime).clientRuntime'></a>

`clientRuntime` [System.ServiceModel.Dispatcher.ClientRuntime](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Dispatcher.ClientRuntime 'System.ServiceModel.Dispatcher.ClientRuntime')

The client runtime to be customized.

Implements [ApplyClientBehavior(ServiceEndpoint, ClientRuntime)](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Description.IEndpointBehavior.ApplyClientBehavior#System_ServiceModel_Description_IEndpointBehavior_ApplyClientBehavior_System_ServiceModel_Description_ServiceEndpoint,System_ServiceModel_Dispatcher_ClientRuntime_ 'System.ServiceModel.Description.IEndpointBehavior.ApplyClientBehavior(System.ServiceModel.Description.ServiceEndpoint,System.ServiceModel.Dispatcher.ClientRuntime)')