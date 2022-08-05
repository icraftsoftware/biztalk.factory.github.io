#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfNetNamedPipeAdapter](WcfNetNamedPipeAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter')

## WcfNetNamedPipeAdapter.Inbound Class

The WCF-NetNamedPipe adapter provides cross-process communication on the same computer in an environment in which
both services and clients are WCF based. It provides full access to SOAP reliability and transaction features. The
adapter uses the named pipe transport, and messages have binary encoding. This adapter cannot be used in
cross-computer communication.

```csharp
public class WcfNetNamedPipeAdapter.Inbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter<Microsoft.BizTalk.Adapter.Wcf.Config.NetNamedPipeRLConfig>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxConcurrentCalls,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundIncludeExceptionDetailInFaults,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundSuspendRequestMessageOnFailure,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase&lt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.EndpointAddress](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.EndpointAddress 'System.ServiceModel.EndpointAddress')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.Configuration.NetNamedPipeBindingElement](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Configuration.NetNamedPipeBindingElement 'System.ServiceModel.Configuration.NetNamedPipeBindingElement')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.NetNamedPipeRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.NetNamedPipeRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.NetNamedPipeRLConfig')[&gt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase&lt;](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.EndpointAddress](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.EndpointAddress 'System.ServiceModel.EndpointAddress')[,](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.Configuration.NetNamedPipeBindingElement](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Configuration.NetNamedPipeBindingElement 'System.ServiceModel.Configuration.NetNamedPipeBindingElement')[,](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.NetNamedPipeRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.NetNamedPipeRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.NetNamedPipeRLConfig')[&gt;](WcfOneWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOneWayAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase&lt;](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.EndpointAddress](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.EndpointAddress 'System.ServiceModel.EndpointAddress')[,](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>')[System.ServiceModel.Configuration.NetNamedPipeBindingElement](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Configuration.NetNamedPipeBindingElement 'System.ServiceModel.Configuration.NetNamedPipeBindingElement')[,](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.NetNamedPipeRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.NetNamedPipeRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.NetNamedPipeRLConfig')[&gt;](WcfTwoWayAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfTwoWayAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter&lt;](WcfNetNamedPipeAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter<TConfig>')[Microsoft.BizTalk.Adapter.Wcf.Config.NetNamedPipeRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Wcf.Config.NetNamedPipeRLConfig 'Microsoft.BizTalk.Adapter.Wcf.Config.NetNamedPipeRLConfig')[&gt;](WcfNetNamedPipeAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter<TConfig>') &#129106; Inbound

Implements [IInboundAdapter](IInboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation'), [IAdapterConfigMaxConcurrentCalls](IAdapterConfigMaxConcurrentCalls.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxConcurrentCalls'), [IAdapterConfigInboundIncludeExceptionDetailInFaults](IAdapterConfigInboundIncludeExceptionDetailInFaults.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundIncludeExceptionDetailInFaults'), [IAdapterConfigInboundSuspendRequestMessageOnFailure](IAdapterConfigInboundSuspendRequestMessageOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigInboundSuspendRequestMessageOnFailure'), [IAdapterConfigSSO](IAdapterConfigSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO')

### See Also
- [What Is the WCF-NetNamedPipe Adapter?](https://docs.microsoft.com/en-us/biztalk/core/what-is-the-wcf-netnamedpipe-adapter 'https://docs.microsoft.com/en-us/biztalk/core/what-is-the-wcf-netnamedpipe-adapter')
- [How to Configure a WCF-NetNamedPipe Receive Location](https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-a-wcf-netnamedpipe-receive-location 'https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-a-wcf-netnamedpipe-receive-location')
- [WCF-NetNamedPipe Transport Properties Dialog Box, Receive, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-netnamedpipe-transport-properties-dialog-box-receive-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-netnamedpipe-transport-properties-dialog-box-receive-security-tab')
- [WCF
            Adapters Property Schema and Properties](https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters-property-schema-and-properties 'https://docs.microsoft.com/en-us/biztalk/core/wcf-adapters-property-schema-and-properties')

| Constructors | |
| :--- | :--- |
| [Inbound()](WcfNetNamedPipeAdapter.Inbound.Inbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter.Inbound.Inbound()') | |
| [Inbound(Action&lt;Inbound&gt;)](WcfNetNamedPipeAdapter.Inbound.Inbound(Action_Inbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter.Inbound.Inbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter.Inbound>)') | |

| Properties | |
| :--- | :--- |
| [IncludeExceptionDetailInFaults](WcfNetNamedPipeAdapter.Inbound.IncludeExceptionDetailInFaults.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter.Inbound.IncludeExceptionDetailInFaults') | |
| [MaxConcurrentCalls](WcfNetNamedPipeAdapter.Inbound.MaxConcurrentCalls.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter.Inbound.MaxConcurrentCalls') | |
| [SuspendRequestMessageOnFailure](WcfNetNamedPipeAdapter.Inbound.SuspendRequestMessageOnFailure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter.Inbound.SuspendRequestMessageOnFailure') | |
| [UseSSO](WcfNetNamedPipeAdapter.Inbound.UseSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfNetNamedPipeAdapter.Inbound.UseSSO') | |