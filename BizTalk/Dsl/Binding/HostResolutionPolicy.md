# Host Resolution Policy

> **Downloads** The code samples used in this user guide have been made available in the [Be.Stateless.BizTalk.Factory.Samples][github.samples] GitHub repository.

There usually are conventions when defining Microsoft BizTalk Server® hosts and host instances. It is a [standard practice][biztalk-host-recommendation] to at least create different hosts for processing, receiving, or sending purposes. But one could also chose to create a host by available adapters and directions. Host conventions could also be influenced by network zones, or DMZ, where some adapters could only be available in only one zone, while some others might be available in multiple zones. Some adapters further require to be hosted in an isolated process. Moreover, hosts might not be configured the same way in all target deployment environments, for instance; it usually is the case that the `DEVELOPMENT` and `BUILD` environments have different host configurations than the `ACCEPTANCE` and `PRODUCTION` environments &mdash;though one should strive to have identical host configurations for the `ACCEPTANCE` and `PRODUCTION` environments.

The Microsoft BizTalk Server® host conventions can consequently be quite elaborated and binding a port artifact to its right host can become error-prone. Instead of leaving the responsibility entirely to the developer to pick the right host &mdash;usually a `string` literal name&mdash; when configuring an artifact, one could write a policy that would automatically resolve the right host to bind the artifact to, as in the following code

```csharp
Transport.Host = Host.Default
```

instead of the traditional explicit host name assignment

```csharp
Transport.Host = "BizTalkServerApplication"
```

> **Remark** Both expressions above are supported by `BizTalk.Factory`'s `Binding DSL` out of the box, i.e. assigning either a `string` literal or a policy object.

The corner stone of the host resolution policy mechanism is the [ISupportHostResolution][i-support-host-resolution] interface together combined with the [HostResolutionPolicy][host-resolution-policy-base] base class policy, which is the policy that accepts any `string` literal as the host name to be resolved when the bindings will be generated for whatever target deployment environment.

`BizTalk.Factory` also comes with an additional [HostResolutionPolicy][host-resolution-policy-convention] that matches the default Microsoft BizTalk Server® host setup &mdash;`BizTalkServerApplication` and `BizTalkServerIsolatedHost` hosts&mdash; and automatically picks the right host among the isolated or in-process ones for a receive location. This is the policy that a developer would typically use for the `DEVELOPMENT` or `BUILD` target deployment environments.

If the developer needs to provide a richer host resolution policy, he can write a custom class that derives from the [HostResolutionPolicy][host-resolution-policy-base] base policy, override the members according to his needs, and finally bind &mdash;assign&mdash; an instance of this custom policy to any orchestration or transport host.

## Sample

For the sake of illustration, let us imagine that the developer needs to write a policy that will resolve the right host according to the following rules:

- Following the [standard practice][biztalk-host-recommendation], distinct hosts will be created according to their processing, receiving, sending, or tracking role;

- Each Microsoft BizTalk Server® adapter will have a dedicated host;

- An adapter will _generally_ be supported in only one of the two `Intranet` or `B2B` network zones &mdash;it would be rather inefficient and illogical to host an `SFTP` adapter in the `Intranet` zone,&mdash; while some adapters, like the `WcfWebHttpAdapter`, might reside in both network zones.\
  Besides, if an adapter can be hosted in multiple network zones, the latter must be explicitly chosen by the developer or the generation of the application bindings should fail.

- To avoid the burden of operating a Microsoft BizTalk Server® cluster, inbound adapters that cannot be hosted in concurrent host instances will have to be hosted on one single host instance &mdash;e.g. `Pop3Adapter.Inbound` or `SftpAdapter.Inbound`;

- Some adapters finally require either or both a 32-bit or an isolated process.

The following pattern integrates and summarizes all the above constraints:

```
<L|P|R|T>xHost[_B2B][_<Adapter>][_32][_Single]
```

where

- `<L|P|R|T>` respectively denotes whether it is an isolated, processing, receiving or sending host;
- `B2B` denotes that this host has instances running either in the `B2B` network zone, if present, or in the `Intranet` network zone, if absent;
- `<Adapter>` denotes a host that is dedicated to a single adapter, e.g. `File`, `WcfSql` &mdash;this token is obviously not relevant for processing hosts;
- `32` denotes that this host has 32-bit instances, if present, or 64-bit instances, if absent;
- `Single` denotes that this host has a single instance, if present, or multiple instances, if absent &mdash;this token is only relevant for host running inbound adapters that do not support concurrency.

The sample `Org.Anization.BizTalk.Environment.Settings` project provides a host resolution policy &mdash;[AnyNetworkZoneHostResolutionPolicy][any-network-zone-host-resolution-policy] accessible via its factory [Host][host-factory] singleton&mdash; that satisfies all these requirements and allows the developer to bind a Microsoft BizTalk Server® artifact to a host as follows:

```csharp
using Org.Anization.BizTalk.Environment.Settings;

Transport.Host = Host.Default;

Transport.Host = Host.Intranet;

Transport.Host = Host.B2B;
```

In order to implement the [AnyNetworkZoneHostResolutionPolicy][any-network-zone-host-resolution-policy] host resolution policy, some amount of scaffolding code has been written; this code is provided with unit tests that also shed some light on its purpose and how to use it. At the basis of it all, there are the [NetworkZones][network-zones] enumeration and the [AdapterExtensions][adapter-extensions] class. The former defines the network zones that will be supported by the policy, the latter provides some extension methods to [IAdapter][i-adapter]-derived classes that allows to determine some of its characteristics, as for instance its name or whether it is a `WCF`-based adapter, etc.

Built on top of these, then come the [InboundAdapterExtensions][inbound-adapter-extensions] and [OutboundAdapterExtensions][outbound-adapter-extensions] classes, whose role is to determine whether an adapter is supported in any given network zone &mdash;the classes contain decision tables with an entry for each of the adapter configuration classes provided by `BizTalk.Factory`'s `Binding DSL`. Notice that `WCF`-based adapters can be equivalently configured in two different ways, either through their explicit configuration classes, e.g. `WcfBasicHttpAdapter.Outbound`, or through the generic `WcfCustomAdapter.Outbound<>` configuration class, e.g. `WcfCustomAdapter.Outbound<BasicHttpBindingElement>`. It would be a resource waste to host equivalent `WCF`-based adapters in two different processes just because they have been configured through their explicit or generic configuration classes. In order to avoid multiple similar entries in the decision tables concerning `WCF` adapters, it is therefore not the actual adapter configuration class but its binding element that is used.

The following table summarizes the hosts that will be available in each network zone to support the adapters, as implemented by the previously mentioned decision tables:

| Adapter           | Isolated | Inbound  | Outbound |
| ----------------- | -------- | -------- | -------- |
| File              | -        | Intranet | Intranet |
| FTP               | -        | None     | None     |
| HTTP              | -        | Intranet | All      |
| Office365Email    | -        | B2B      | -        |
| POP3              | -        | B2B      | -        |
| SBMessaging       | -        | B2B      | B2B      |
| SFTP              | -        | B2B      | B2B      |
| WcfBasicHttp      | All      | None     | All      |
| WcfBasicHttpRelay | None     | None     | None     |
| WcfNetMsmq        | None     | Intranet | Intranet |
| WcfNetNamedPipe   | None     | None     | All      |
| WcfNetTcp         | Intranet | Intranet | Intranet |
| WcfNetTcpRelay    | None     | None     | None     |
| WcfOracle         | None     | Intranet | Intranet |
| WcfSap            | None     | Intranet | Intranet |
| WcfSql            | None     | Intranet | Intranet |
| WcfWebHttp        | All      | None     | All      |
| WcfWSHttp         | B2B      | None     | B2B      |

With this knowledge in place, [NetworkZoneBoundHostResolutionPolicy][network-zone-bound-host-resolution-policy] is the last scaffolding class that we need in order to compute the name of the host that will actually run a Microsoft BizTalk Server® artifact. This latter class has to be instantiated for each network zone that we care to support. And that is precisely what [AnyNetworkZoneHostResolutionPolicy][any-network-zone-host-resolution-policy] does, combined with the fact that the latter will throw when a host is available in multiple network zones so as to require the developer to remove the ambiguity &mdash;instead of assigning `Host.Default`, the developer will have to either pick `Host.Intranet` or `Host.B2B`.

<!-- links -->

[github.samples]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples

<!--  -->

[adapter-extensions]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples/blob/master/src/Org.Anization.BizTalk.Environment.Settings/Environment/Settings/Convention/Extensions/AdapterExtensions.cs
[any-network-zone-host-resolution-policy]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples/blob/master/src/Org.Anization.BizTalk.Environment.Settings/Environment/Settings/Convention/AnyNetworkZoneHostResolutionPolicy.cs
[biztalk-host-recommendation]: https://docs.microsoft.com/en-us/biztalk/technical-guides/high-availability-for-biztalk-hosts
[host-factory]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples/blob/master/src/Org.Anization.BizTalk.Environment.Settings/Environment/Settings/Host.cs
[host-resolution-policy-base]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Convention/HostResolutionPolicy.cs
[host-resolution-policy-convention]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding.Conventions/Factory/Convention/HostResolutionPolicy.cs
[i-adapter]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Adapter/IAdapter.cs
[i-support-host-resolution]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Convention/ISupportHostResolution.cs
[inbound-adapter-extensions]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples/blob/master/src/Org.Anization.BizTalk.Environment.Settings/Environment/Settings/Convention/Extensions/InboundAdapterExtensions.cs
[network-zone-bound-host-resolution-policy]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples/blob/master/src/Org.Anization.BizTalk.Environment.Settings/Environment/Settings/Convention/NetworkZoneBoundHostResolutionPolicy.cs
[network-zones]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples/blob/master/src/Org.Anization.BizTalk.Environment.Settings/Environment/Settings/NetworkZones.cs
[outbound-adapter-extensions]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples/blob/master/src/Org.Anization.BizTalk.Environment.Settings/Environment/Settings/Convention/Extensions/OutboundAdapterExtensions.cs

<!--
cSpell:ignore Anization msmq
-->
