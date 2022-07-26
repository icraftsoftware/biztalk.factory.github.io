# Adapter Binding

> **Downloads** The code samples used in this user guide have been made available in the [Be.Stateless.BizTalk.Factory.Samples][github.samples] GitHub repository.

## Available Adapters

The namespace `Be.Stateless.BizTalk.Dsl.Binding.Adapter` provides a rich set of adapter configuration classes &mdash;e.g. `FileAdapter` or `WcfSqlAdapter`. Every such class furthermore nests either or both an inbound and outbound classes &mdash;e.g. `FileAdapter.Inbound` or `WcfSqlAdapter.Outbound`&mdash; that surface the actual configuration properties of respectively the inbound or outbound adapter.

As detailed in the following table, `BizTalk.Factory`'s `Binding DSL` currently supports most of the built-in Microsoft BizTalk Server® adapters:

| Adapter                            | Inbound | Outbound | [Deprecated][deprecated-adapters] |
| ---------------------------------- | ------- | -------- | --------------------------------- |
| `AzureBlobStorageAdapter`          | &cross; | &cross;  |                                   |
| `EventHubAdapter`                  | &cross; | &cross;  |                                   |
| `FileAdapter`                      | &check; | &check;  |                                   |
| `FtpAdapter`                       | &check; | &check;  |                                   |
| `HttpAdapter`                      | &check; | &check;  |                                   |
| `LogicAppAdapter`                  | &cross; | &cross;  |                                   |
| `MQSeriesAdapter`                  | &cross; | &cross;  |                                   |
| `MsmqAdapter`                      | &cross; | &cross;  |                                   |
| `Office365CalendarAdapter`         | &cross; | &cross;  |                                   |
| `Office365ContactAdapter`          | &cross; | &cross;  |                                   |
| `Office365EmailAdapter`            | &check; | &cross;  |                                   |
| `Pop3Adapter`                      | &check; | -        | &check;                           |
| `SBMessagingAdapter`               | &check; | &check;  |                                   |
| `SharePointOnlineAdapter`          | &cross; | &cross;  |                                   |
| `SftpAdapter`                      | &check; | &check;  |                                   |
| `SmtpAdapter`                      | -       | &cross;  | &check;                           |
| `SoapAdapter`                      | &cross; | &cross;  | &check;                           |
| `SqlAdapter`                       | &cross; | &cross;  | &check;                           |
| `WcfBasicHttpAdapter`              | &check; | &check;  |                                   |
| `WcfBasicHttpRelayAdapter`         | &check; | &check;  |                                   |
| `WcfCustomAdapter`                 | &check; | &check;  |                                   |
| `WcfCustomIsolatedAdapter`         | &check; | -        |                                   |
| `WcfNetMsmqAdapter`                | &check; | &check;  |                                   |
| `WcfNetNamedPipeAdapter`           | &check; | &check;  |                                   |
| `WcfNetTcpAdapter`                 | &check; | &check;  |                                   |
| `WcfNetTcpRelayAdapter`            | &check; | &check;  | &check;                           |
| `WcfOracleAdapter`                 | &check; | &check;  |                                   |
| `WcfOracleEBusinessAdapter`        | &cross; | &cross;  |                                   |
| `WcfSapAdapter`                    | &check; | &check;  |                                   |
| `WcfSiebelAdapter`                 | &cross; | &cross;  |                                   |
| `WcfSqlAdapter`                    | &check; | &check;  |                                   |
| `WcfWebHttpAdapter`                | &check; | &check;  |                                   |
| `WcfWSHttpAdapter`                 | &check; | &check;  |                                   |
| `WindowsSharePointServicesAdapter` | &cross; | &cross;  |                                   |

> **Remark** The vast majority of the adapter configuration classes provided by `Be.Stateless.BizTalk.Dsl.Binding` is a delegation `API` that taps right into the [System.ServiceModel.Configuration.StandardBindingElement][standard-binding-element]-derived classes or other Microsoft BizTalk Server® native configuration classes. The developer should therefore feel confident that the configuration bindings produced by `BizTalk.Factory`'s `Binding DSL` are truly accurate and faithful to any actual Microsoft BizTalk Server® application bindings that would be produced otherwise.

## `WCF`-based Adapters

`WCF`-based adapters typically provide many highly customizable features. Since `WCF` was built as a `SOAP` stack, these adapters therefore present a configuration `API` which exposes core `SOAP` concepts. Among them, we will retain actions, bindings, and behaviors, which are customization areas that deserve further in-depth treatment.

### `SOAP` Action Configuration

#### Action Mapping

`SOAP` action configuration is performed through the `StaticAction` property of the adapter &mdash;see the [IAdapterConfigOutboundAction][i-adapter-config-outbound-action] interface. Even though the `StaticProperty` is a simple `string`, it can either be configured to a single `SOAP` action literal:

```csharp
adapter.StaticAction = "http://services.stateless.be/biztalk/factory/mail/1.1/IMailService/SendMessage";
```

or to a set of mappings from Microsoft BizTalk Server® operations to `SOAP` action literals:

```csharp
using Be.Stateless.BizTalk.Adapter.Metadata;

...

adapter.StaticAction = new ActionMapping {
  new ActionMappingOperation(
    "UpdateIntervention",
    "http://Microsoft.LobServices.OracleDB/2007/03/TICKETING/Procedure/UPDATE_INTERVENTION"),
  new ActionMappingOperation(
    "UpdateOperation",
    "http://Microsoft.LobServices.OracleDB/2007/03/TICKETING/Procedure/UPDATE_OPERATION")
};
```

> **Remark** If you use JetBrains [ReSharper][resharper] you can get the `StaticAction` quick help as a reminder on how to configure the property, as illustrated [here][quich-help-static-action].\
> Press <kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>F1</kbd> with the caret inside the lexical token for which you want to get the help; in this case, `StaticAction`.

#### `HTTP` Methods and `URL` Mapping

Though meant to provide `REST`ful interactions through parameterized `URL`s and `HTTP` methods &mdash;which somehow are to `REST` what actions are to `SOAP`,&mdash; the `WcfWebHttpAdapter` adapter has been built on top of `WCF`, which is `SOAP` centric. The `WCF` stack and configuration model therefore had to be twisted to support the feature set of `REST`ful interactions and, as a result, idiosyncratic configuration properties such as `HttpUrlMapping`, `VariableMapping`, and `SuppressMessageBodyForHttpVerbs`, surfaced through the configuration `API` of the `WcfWebHttpAdapter`.

```csharp
Transport.Adapter = new WcfWebHttpAdapter.Outbound(
   a => {
      a.Address = new EndpointAddress($"http://{Application.Settings.ApiHost}/api");
      a.HttpHeaders = "Content-Type: application/xml\r\n"
         + "Accept: application/xml";
      a.HttpUrlMapping = new HttpUrlMapping {
         new HttpUrlMappingOperation(
            Processes.Declare.ProcessOrchestrationBinding.RequestApiPort.Operations.GetRequest.Name,
            HttpMethod.Get.Method,
            $"/v1/request/{{{QueryParameterProperties.RequestId.Name}}}")
      };
      a.SuppressMessageBodyForHttpVerbs = HttpMethod.Get.Method;
      a.VariableMapping = new VariableMapping {
         new VariablePropertyMapping(QueryParameterProperties.RequestId.Name, QueryParameterProperties.RequestId)
      };
      a.EndpointBehaviors = new BehaviorExtensionElement[] {
         new WebHttpElement { FaultExceptionEnabled = true },
         new WebHttpAuthorizationBehaviorExtension {
            AuthorizationTokenServiceMiddlewareType = typeof(AuthorizationTokenServiceMiddleware),
            AuthorizationTokenServiceUri = $"http://{Application.Settings.ApiHost}/api/token/service"
         },
         new WebHttpErrorInspectionBehaviorExtension()
      };
});
```

### `WCF` Behavior Configuration

How a `WCF`-based adapter actually interacts with its counterpart at runtime can be customized thanks to behavior components which will be injected in the communication channel at construction time. Depending on whether the `WCF` exposes or consumes an endpoint, behavior customization is respectively surfaced through either the `ServiceBehaviors` or the `EndpointBehaviors` property. An example of how to configure the `EndpointBehaviors` has been provided in the previous code excerpt.

> **Remark** Even though every `WCF` communication channel can be an injection site for custom behavior components, most of the Microsoft BizTalk Server® built-in `WCF`-based adapters do not allow injecting custom behavior components but come with predefined ones. As a result, the `WCF` channel per se is not customizable, but the individual behavior components are.
>
> To customize the `WCF` channel the developer therefore has no other choice than to fall-back on the `WcfCustomAdapter` or `WcfCustomIsolatedAdapter` and reconfigure the whole channel according to the binding &mdash;`HTTP`, `net.tcp`, `WSHttp`&mdash; he whishes to use.
>
> Microsoft BizTalk Server® LOB Adapters such as `WcfOracleAdapter`,`WcfSapAdapter`, or `WcfSqlAdapter`, as well as the `WcfWebHttpAdapter` are noticeable exceptions that always allow the `WCF` channel to be customized with behavior components.

### `WCF` Binding Configuration

The `WCF` binding is the actual transport, such as `HTTP`, being used to connect to an endpoint &mdash;technically a binding can define much more than the transport as explained [here][wcf-binding]. For Microsoft BizTalk Server® `WCF`-based adapters, the binding configuration is performed through the `Binding` property of the adapter &mdash;see the [IAdapterConfigBinding&lt;T&gt;][i-adapter-config-binding] interface. As most of the Microsoft BizTalk Server® adapters assumes a predefined transport, only the `WcfCustomAdapter` and `WcfCustomIsolatedAdapter` adapter support binding configuration.

How to configure an inbound `WcfCustomAdapter` is illustrated in the following code excerpt. Notice that the binding denoting the transport to use, i.e. `NetTcpBindingElement`, is given as a generic type argument and that is the actual `WCF` binding element configuration class and not a custom wrapper provided by `BizTalk.Factory`.

```csharp
const int tenMegaBytes = 10 * 1024 * 1024;

Transport.Adapter = WcfCustomAdapter.Inbound<NetTcpBindingElement>(
   a => {
         a.Address = new EndpointAddress("net.tcp://localhost/biztalk.factory/service.svc");
         a.Binding.MaxReceivedMessageSize = tenMegaBytes;
         a.Binding.ReaderQuotas.MaxArrayLength = tenMegaBytes;
         a.Binding.ReaderQuotas.MaxStringContentLength = tenMegaBytes;
         a.Binding.Security.Mode = SecurityMode.Transport;
         a.Binding.Security.Transport.ProtectionLevel = ProtectionLevel.Sign;
         a.Binding.Security.Transport.ClientCredentialType = TcpClientCredentialType.Windows;
         a.OpenTimeout = TimeSpan.FromMinutes(3);
});
```

## Advanced Configuration Scenario

As you have seen in the [Environment Overrides](./README.md#environment-overrides) section, `BizTalk.Factory`'s `Binding DSL` supports multiple target deployment environments. Suppose that in the development and build environments you need to use a given transport, let us say `HTTP` &mdash;the stub you are using for testing purposes only supports `HTTP`&mdash; but in acceptance and production environments you have to use another transport, let us say `net.tcp`. Let us suppose further that you want to share the same action mapping and behavior configuration in all the environments to make sure the `WCF` channel and the Microsoft BizTalk Server® interaction flows will behave as expected.

As we saw earlier, configuring the behaviors requires to fall back on a `WcfCustomAdapter`. The following code sample illustrates how one could share the configuration commonalities between the various target deployment environments:

```csharp
class IrsSendPort : SendPort<NamingConvention>
{
   public IrsSendPort()
   {
      Name = SendPortName.Towards("Irs").About("Anything").FormattedAs.Irrelevant;
      SendPipeline = new SendPipeline<PassThruTransmit>();
      ReceivePipeline = new ReceivePipeline<PassThruReceive>();
      var adapter = new WcfCustomAdapter.Outbound<BasicHttpBindingElement>(
         a => {
            a.Address = new EndpointAddress("http://localhost/soap-stub");
            a.Binding.MaxReceivedMessageSize = tenMegaBytes;
         });
      Transport.Adapter = ApplyAdapterCommonalities(adapter);
      Transport.Host = DummyHostResolutionPolicy.Default;
   }

   protected override void ApplyEnvironmentOverrides(string environment)
   {
      if (environment.IsAcceptanceUpwards())
      {
         var adapter = new WcfCustomAdapter.Outbound<NetTcpBindingElement>(
            a => {
               a.Address = new EndpointAddress("net.tcp://host/api/services/");
               a.Binding.MaxReceivedMessageSize = tenMegaBytes;
               a.Binding.Security.Mode = SecurityMode.Transport;
               a.Binding.Security.Transport.ClientCredentialType = TcpClientCredentialType.Windows;
               a.Binding.Security.Transport.ProtectionLevel = ProtectionLevel.EncryptAndSign;
            });
         Transport.Adapter = ApplyAdapterCommonalities(adapter);
      }
   }

   private IOutboundAdapter ApplyAdapterCommonalities<TAdapter>(TAdapter adapter)
      where TAdapter : IOutboundAdapter, IAdapterConfigEndpointBehavior, IAdapterConfigOutboundAction
   {
      adapter.EndpointBehaviors = new BehaviorExtensionElement[] {
         new CallbackDebugElement()
      };
      adapter.StaticAction = new ActionMapping {
         new ActionMappingOperation("operation", "action")
      };
      return adapter;
   }
}
```

Notice that the `ApplyAdapterCommonalities` method could have the following signature instead without any impact on the `C#` code and its semantics:

```csharp
private IOutboundAdapter ApplyAdapterCommonalities<TBinding>(WcfCustomAdapter.Outbound<TBinding> adapter)
	where TBinding : StandardBindingElement, new()
```

The careful reader will have noticed that the `ApplyAdapterCommonalities` method does not handle the `a.Binding.MaxReceivedMessageSize`. The actual reason is that there is no common interface nor any common base class among `BasicHttpBindingElement` and `NetTcpBindingElement` &mdash;both directly inherit from `StandardBindingElement`&mdash; that define the `MaxReceivedMessageSize` property.

If the developer did not need to customize the behaviors, then he could have written the following code instead &mdash;but would be **totally** incapable of customizing the behaviors:

```csharp
class SomePartySendPort : SendPort<NamingConvention>
{
   public SomePartySendPort()
   {
      Name = SendPortName.Towards("SomeParty").About("Anything").FormattedAs.Xml;
      SendPipeline = new SendPipeline<PassThruTransmit>();
      var adapter = new WcfBasicHttpAdapter.Outbound(a => { a.Address = new EndpointAddress("http://localhost/soap-stub"); });
      Transport.Adapter = ApplyAdapterCommonalities(adapter);
      Transport.Host = DummyHostResolutionPolicy.Default;
   }

   [SuppressMessage("ReSharper", "InvertIf")]
   protected override void ApplyEnvironmentOverrides(string environment)
   {
      if (environment.IsAcceptanceUpwards())
      {
         var adapter = new WcfNetTcpAdapter.Outbound(
            a => {
               a.Address = new EndpointAddress("net.tcp://host/api/services/");
               a.Identity = new IdentityElement { ServicePrincipalName = { Value = "spn" } };
               a.SecurityMode = SecurityMode.Transport;
               a.TransportClientCredentialType = TcpClientCredentialType.Windows;
               a.TransportProtectionLevel = ProtectionLevel.EncryptAndSign;
            });
         Transport.Adapter = ApplyAdapterCommonalities(adapter);
      }
   }

   private IOutboundAdapter ApplyAdapterCommonalities<TAdapter>(TAdapter adapter)
      where TAdapter : IOutboundAdapter, IAdapterConfigMaxReceivedMessageSize, IAdapterConfigOutboundAction
   {
      adapter.MaxReceivedMessageSize = tenMegaBytes;
      adapter.StaticAction = new ActionMapping {
         new ActionMappingOperation("operation", "action")
      };
      return adapter;
   }
}
```

<!-- TODO
   ## Extensibility Points
 -->

<!-- links -->

[github.samples]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples
[deprecated-adapters]: https://docs.microsoft.com/en-us/biztalk/install-and-config-guides/whats-new-in-biztalk-server-2020#deprecated--removed-list
[i-adapter-config-binding]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Adapter/IAdapterConfigBinding.cs
[i-adapter-config-outbound-action]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Adapter/IAdapterConfigOutboundAction.cs
[quich-help-static-action]: ../../../assets/images/QuickHelp.StaticAction.png
[resharper]: https://www.jetbrains.com/resharper/
[standard-binding-element]: https://docs.microsoft.com/en-us/dotnet/api/system.servicemodel.configuration.standardbindingelement
[wcf-binding]: https://docs.microsoft.com/en-us/dotnet/framework/wcf/bindings-overview

<!--
cSpell:ignore biztalk Msmq Siebel typeof
-->
