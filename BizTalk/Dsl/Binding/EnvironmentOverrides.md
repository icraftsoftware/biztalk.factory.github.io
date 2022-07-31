# Environment Overrides

> **Downloads** The code samples used in this user guide have been made available in the [Be.Stateless.BizTalk.Factory.Samples][github.samples] GitHub repository.

A Microsoft BizTalk Server® application generally targets multiple deployment environments, each with a different configuration. The basic use cases for parameterized deployments is that there usually is a set of properties whose value differs in each environment &mdash;e.g. login, passwords, URLs, and so on. This use case is handled and supported via the [Environment Dependent Values](./EnvironmentDependentValues.md), as explained in the following section.

Besides supporting different configurations at the property level, `BizTalk.Factory`'s `Binding DSL` also recognizes scenarios where one application needs to connect to endpoints varying according to the target deployment environment. For instance, when deployed to the _development_ or _build_ environments, some ports would need to be bound to stub endpoints in order for the application's flows to be automatically tested, while some other ports &mdash;e.g. supplementary receive locations belonging to one receive port&mdash; would not need to be deployed at all.

`BizTalk.Factory`'s `Binding DSL` supports this overriding mechanisms through the [ISupportEnvironmentOverride][i-support-environment-override] interface, which provides one single method:

```csharp
void ApplyEnvironmentOverrides(string environment);
```

where the `environment` parameter is a `string` identifying the target deployment environment, i.e. the environment for which the bindings are currently being generated, thus giving an opportunity to each class that supports this interface to adapt its binding configuration accordingly. To be accurate, all the following **base** classes support the [ISupportEnvironmentOverride][i-support-environment-override] interface:

- [ApplicationBindingBase][application-binding-base],
- [OrchestrationBindingBase][orchestration-binding-base],
- [ReceivePortBase][receive-port-base],
- [ReceiveLocationBase][receive-location-base],
- [SendPortBase][send-port-base],
- [TransportBase][transport-base].

and have been provided with a default implementation _similar_ to what follows:

```csharp
void ISupportEnvironmentOverride.ApplyEnvironmentOverrides(string environment)
{
   if (!environment.IsNullOrEmpty()) ApplyEnvironmentOverrides(environment);
}

protected virtual void ApplyEnvironmentOverrides(string environment) { }
```

whose purpose is clearly to free the developer from worrying about nothing else than to provide an `ApplyEnvironmentOverrides` method override when necessary.

> **Remark** The reason the interface has been implemented explicitly and that it delegates the call to a **protected** overridable &mdash;i.e. virtual&mdash; method, with the exact same signature, was not to clutter the Visual Studio® intellisense, which `BizTalk.Factory`'s `Binding DSL` embraced as a way to offer a [fluent interface][fluent-interface] &mdash;exposing only useful and guiding methods and hiding others.

For the sake of completeness, a few of these base classes actually do more than delegating the call to an empty method, they do forward the call to their constituent parts as well.

- The `ReceiveLocationBase` class also forwards the call to its `Transport`;

- The `SendPortBase` class also forwards the call to its `Filter`, `Transport`, and `BackupTransport`.

- The `TransportBase` class has been derived into both a [ReceiveLocationTransport][receive-location-transport] and a [SendPortTransport][send-port-transport], which are respectively the actual transport type of a `ReceiveLocationBase` or a `SendPortBase` class. This distinction allows for each actual `TransportBase`-derived class to forward the `ApplyEnvironmentOverrides` call to its constituent parts.

  - The `ReceiveLocationTransport` forwards the call to its `Schedule`;
  - The `SendPortTransport` forwards the call to its `RetryPolicy` and `ServiceWindow`.

While, as we have seen, the endpoints to which to connect could vary with the target deployment environments, a port, on the contrary, should share as much features and configuration as possible across its target deployment environments. Failure to do so so would make an application hardly predictable and seriously reduce the value of the automated tests. What could we conclude from automated tests if a port's pipelines or adapter were configured differently in each deployment environment? For these reasons, `BizTalk.Factory`'s `Binding DSL` does not support `ApplyEnvironmentOverrides` call forwarding for the following port's constituent:

- [ReceivePipeline][receive-pipeline],
- [SendPipeline][send-pipeline],
- [AdapterBase][adapter-base].

<!-- links -->

[github.samples]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples

<!--  -->

[adapter-base]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Adapter/AdapterBase.cs
[application-binding-base]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/ApplicationBindingBase.cs
[fluent-interface]: https://github.com/kzu/IFluentInterface#readme
[i-support-environment-override]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/ISupportEnvironmentOverride.cs
[orchestration-binding-base]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/OrchestrationBindingBase.cs
[receive-location-base]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/ReceiveLocationBase.cs
[receive-location-transport]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/ReceiveLocationTransport.cs
[receive-pipeline]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/ReceivePipeline.cs
[receive-port-base]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/ReceivePortBase.cs
[send-pipeline]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/SendPipeline.cs
[send-port-base]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/SendPortBase.cs
[send-port-transport]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/SendPortTransport.cs
[transport-base]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/TransportBase.cs

<!--
cSpell:ignore overridable
-->
