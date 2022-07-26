# Orchestration Binding

> **Downloads** The code samples used in this user guide have been made available in the [Be.Stateless.BizTalk.Factory.Samples][github.samples] GitHub repository.

To better support the binding of Microsoft BizTalk Server® orchestrations, `BizTalk.Factory`'s `Binding DSL` needs the combined work of the [BizTalk.Server.2020.Build][biztalk.server.2020.build] `NuGet` package, which customizes the `MSBuild` process to generate scaffolding `C#` code providing strongly-typed orchestration classes &mdash;see [Be.Stateless.BizTalk.Build.Tasks](../../Build/Tasks/README.md). As soon as both the [BizTalk.Server.2020.Build][biztalk.server.2020.build] `NuGet` package and the project containing the orchestrations are referenced by the application binding configuration project, a custom `MSBuild` task will generate a `<namespace>\<namespace>\<orchestration>OrchestrationBinding.Designer.cs` file for each orchestration found in the referenced project.

For an orchestration whose full name is `Be.Stateless.BizTalk.Orchestrations.Process`, the generated code will be similar to what follows:

```csharp
namespace Be.Stateless.BizTalk.Orchestrations
{
  using System;
  using System.CodeDom.Compiler;
  using Be.Stateless.BizTalk.Dsl.Binding;
  using Microsoft.XLANGs.Core;

  [GeneratedCodeAttribute("Be.Stateless.BizTalk.Build.Tasks", "2.1.0.0")]
  internal partial interface IProcessOrchestrationBinding : IOrchestrationBinding
  {
    IReceivePort RequestResponsePort { get; set; }
    ISendPort SolicitResponsePort { get; set; }
  }

  [GeneratedCodeAttribute("Be.Stateless.BizTalk.Build.Tasks", "2.1.0.0")]
  internal partial class ProcessOrchestrationBinding : OrchestrationBindingBase<Process>, IProcessOrchestrationBinding
  {
    public struct DirectReceivePort
    {
      public struct Operations
      {
        public struct DirectReceiveOperation { public static string Name = "DirectReceiveOperation"; }
      }
    }

    public struct DirectSendPort
    {
      public struct Operations
      {
        public struct DirectSendOperation { public static string Name = "DirectSendOperation"; }
      }
    }

    public struct RequestResponsePort
    {
      public struct Operations
      {
        public struct RequestResponseOperation { public static string Name = "RequestResponseOperation"; }
      }
    }

    public struct SolicitResponsePort
    {
      public struct Operations
      {
        public struct SolicitResponseOperation { public static string Name = "SolicitResponseOperation"; }
      }
    }

    public ProcessOrchestrationBinding() { }

    public ProcessOrchestrationBinding(Action<IProcessOrchestrationBinding> orchestrationBindingConfigurator)
    {
      orchestrationBindingConfigurator(this);
      ((Be.Stateless.BizTalk.Dsl.ISupportValidation)(this)).Validate();
    }

    IReceivePort IProcessOrchestrationBinding.RequestResponsePort { get; set; }

    ISendPort IProcessOrchestrationBinding.SolicitResponsePort { get; set; }
  }
}
```

There are a few remarkable points to notice:

- The orchestration ports that actually need to be bound are declared by an interface &mdash;`IProcessOrchestrationBinding` in our case&mdash; specifically tailored to the orchestration to be bound, and no direct receive or send ports are part of this interface;

- The ports to bind are either `IReceivePort` or `ISendPort` ports, preventing a developer from inadvertently binding a send port to a receive one and vice versa;

- The configuration class allowing to write the orchestration binding, `ProcessOrchestrationBinding`, derives from the generic [`OrchestrationBindingBase<T>`][orchestration-binding-base] class and passe as generic type argument the actual type of the orchestration to bind;

- Every port of the orchestration, whether send or receive, direct or not, is declared as a nested eponymous `struct` that lists all the operations declared at the port.

This generated code allows to write explicit and strongly-type application and orchestration binding code, without ever resorting to magic strings at all, similarly to what follows:

```csharp
public class TwoWaySendPort : SendPort<NamingConvention>
{
  public TwoWaySendPort()
  {
    Name = SendPortName.Towards(...).About(...).FormattedAs.Xml;
    ...
    Transport.Adapter = new WcfWebHttpAdapter.Outbound(
      a => {
        ...
        a.HttpUrlMapping = new HttpUrlMapping {
          new(
            Be.Stateless.BizTalk.Orchestrations.ProcessOrchestrationBinding.SolicitResponsePort.Operations.SolicitResponseOperation.Name,
            HttpMethod.Post.Method,
            "/url/path")
        };
      });
  }
}

public class ApplicationBinding : ApplicationBinding<NamingConvention>
{

  ...

  protected override void ApplyEnvironmentOverrides(string environment)
  {
    Orchestrations.Add(
      new Be.Stateless.BizTalk.Orchestrations.ProcessOrchestrationBinding(
        ob => {
          ob.RequestResponsePort = ReceivePorts.Find<TwoWayReceivePort>();
          ob.SolicitResponsePort = SendPorts.Find<TwoWaySendPort>();
          ob.State = EnvironmentDependentValue
            .ForDevelopmentOrBuild(ServiceState.Unenlisted)
            .ForAcceptance(ServiceState.Started)
            .ForProduction(ServiceState.Unenlisted);
          ob.Host = Host.Default;
        }));
  }
}
```

Because the generated `C#` code is generated anew at each build, it is guaranteed that the code will not compile anymore should an orchestration port or one of its operations be renamed. Also, because it is generated at each build before the `C#` compiler performs its work, it is not necessary to commit the generated code to the source repository &mdash;but it wouldn't matter if unnecessarily/mistakenly committed.

<!-- links -->

[github.samples]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples

<!--  -->

[biztalk.server.2020.build]: https://www.nuget.org/packages/BizTalk.Server.2020.Build
[orchestration-binding-base]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/OrchestrationBindingBase.cs

<!--
cSpell:ignore Configurator struct Unenlisted XLANGs
-->
