# Naming Conventions

> **Downloads** The code samples used in this user guide have been made available in the [Be.Stateless.BizTalk.Factory.Samples][github.samples] GitHub repository.

`BizTalk.Factory` has baked support into its `Binding DSL` for naming Microsoft BizTalk Server® artifacts such as applications, receive ports and locations, and send ports &mdash;see [INamingConvention][i-naming-convention] and [ISupportNameResolution][i-support-name-resolution]&mdash; and comes with a few ready-to-use custom naming conventions too.

Strictly speaking, the [Be.Stateless.BizTalk.Dsl.Binding][nuget] NuGet package provides the support for artifact naming conventions but only comes with one **unstructured** [`string`-only naming convention][application-binding-convention-string], which is the convention that has been used throughout our sample application so far. This allowed us to write binding configuration code as follows, where the name of an artifact can just be any `string` literal:

```csharp
using Be.Stateless.BizTalk.Dsl.Binding;

public class Application : ApplicationBinding
{
   public Application()
   {
      Name = "Accounting";
      ReceivePorts.Add(
         ReceivePort(
            rp => {
               rp.Name = "Billing Receive Port";
               rp.ReceiveLocations.Add(
                  ReceiveLocation(
                     rl => {
                        rl.Name = "Credit Note Receive Location";
      ...
```

The [Be.Stateless.BizTalk.Dsl.Binding.Conventions][nuget.conventions] NuGet package, on the other hand, provides both a [simple][simple-naming-convention] and a [detailed][detailed-naming-convention] **structured** naming conventions. The developer is invited to have a look at sample application bindings making use of the [simple][simple-naming-convention-sample] and [detailed][detailed-naming-convention-sample] naming conventions.

From these samples, there are a few key concepts that one needs to grasp. The actual application binding configuration class the developer writes derives from a base class accepting a naming convention as a generic type argument, see for instance [ApplicationBinding][application-binding-convention-structured]. This base class defines protected factory members that bootstraps the naming convention for any given artifact, e.g. `ApplicationName`, `ReceivePortName`, `ReceiveLocationName`, and `SendPortName`. These factory members allows for the following code to be written, where the name of an artifact can only be assigned a structured expression rooted in one of them:

```csharp
public class SampleApplication : ApplicationBinding<NamingConvention>
{
   public SampleApplication()
   {
      Name = ApplicationName.Is("SampleApplication");
      ReceivePorts.Add(
         ReceivePort(
            rp => {
               rp.Name = ReceivePortName.Offwards("Batch");
               rp.ReceiveLocations.Add(
                  ReceiveLocation(
                     rl => {
                        rl.Name = ReceiveLocationName.About("Release").FormattedAs.Xml;
                        rl.ReceivePipeline = new ReceivePipeline<...>();
                        rl.SendPipeline = new SendPipeline<...>();
                        rl.Transport.Adapter = new WcfSqlAdapter.Inbound(a => { ... });
                     }));
            }));
      SendPorts.Add(new StandaloneSendPort());
   }
}

public class StandaloneSendPort : SendPort<NamingConvention>
{
   public StandaloneSendPort()
   {
      Name = SendPortName.Towards("Job").About("Notification").FormattedAs.Xml;
      SendPipeline = new SendPipeline<...>();
      Transport.Adapter = new FileAdapter.Outbound(a => { ... });
   }
}
```

The artifact names will be computed when the `XML` bindings are generated and it will be expanded according to the following structured pattern for a receive/send port or location:

```
<ApplicationName>.<RP|RL|SP><1|2>.<Party>.<Subject>.<Adapter>.<MessageFormat>
```

where

- `<ApplicationName>` is the application name defined via the convention `API`, i.e. `ApplicationName.Is("Simple.SampleApplication")`;
- `<RP|RL|SP>` respectively denotes either a receive port, a receive location, or a send port;
- `<1|2>` respectively a one-way or two-way port;
- `<Party>` is the party with which the port interacts, i.e. `ReceivePortName.Offwards("Job")` or `SendPortName.Towards("Job")`;
- `<Subject>` denotes what the message is about, i.e. `.About("AddPart")` or `.About("Notification")`;
- `<Adapter>` is the adapter used by the port;
- `<MessageFormat>` is the format of the message payload.

> **Remark** The `<RP|RL|SP>`, `<1|2>`, and `<Adapter>` tokens are automatically computed by the naming convention. For the most cases, the `<Adapter>` token is the name of the adapter, bound to the port's `Transport`, as actually defined in the `Adapters` section underneath the `Platform Settings` of the Microsoft BizTalk Server® Administration Console. Exceptions are made for the `Office365EmailAdapter`, `WcfCustomAdapter`, and `WcfCustomIsolatedAdapter` adapters and details can be found in the source code of the [ComputeAdapterName][naming-convention-compute-adapter-name] method and its [unit tests][naming-convention-compute-adapter-name-tests].

In our case, the naming conventions will produce the following artifact names:

- `SampleApplication` as the application name,
- `SampleApplication.RP2.Batch` for the two-way receive port,
- `SampleApplication.RL2.Batch.Release.WCF-SQL.XML` for the two-way receive location,
- `SampleApplication.SP1.Job.Notification.FILE.XML` for the one-way send port.

Finally, the detailed naming convention is similar to simple one, but furthermore constrains the party &mdash;`OffWards` and `ToWards`&mdash; and subject &mdash;`About`&mdash; names to be defined by some type instead, e.g. an enumeration.

<!-- TODO aggregate token in convention -->

<!-- links -->

[nuget]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Dsl.Binding "Be.Stateless.BizTalk.Dsl.Binding NuGet Package"
[nuget.conventions]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Dsl.Binding.Conventions
[github.samples]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples

<!--  -->

[application-binding-convention-string]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/ApplicationBinding.cs
[application-binding-convention-structured]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding.Conventions/Dsl/Binding/Convention/ApplicationBinding.cs
[detailed-naming-convention-sample]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding.Dummies/Dummies/Bindings/Detailed/SampleApplication.cs
[detailed-naming-convention]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding.Conventions/Dsl/Binding/Convention/Detailed/NamingConvention.cs
[i-naming-convention]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Convention/INamingConvention.cs
[i-support-name-resolution]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Convention/ISupportNameResolution.cs
[naming-convention-compute-adapter-name-tests]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding.Conventions.Tests/Dsl/Binding/Convention/NamingConventionBaseFixture.cs#L58
[naming-convention-compute-adapter-name]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding.Conventions/Dsl/Binding/Convention/NamingConventionBase.cs#L139
[simple-naming-convention-sample]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding.Dummies/Dummies/Bindings/Simple/SampleApplication.cs
[simple-naming-convention]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding.Conventions/Dsl/Binding/Convention/Simple/NamingConvention.cs

<!--
cSpell:ignore offwards
-->
