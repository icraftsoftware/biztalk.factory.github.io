# Be.Stateless.BizTalk.Dsl.Binding

<div class="badges">
<div>

[![][github.badge]][github]

[![][release.badge]][release]

</div>
<div>

[![][pipeline.ci.badge]][pipeline.ci]

[![][pipeline.mr.badge]][pipeline.mr]

</div>
<div>

[![][nuget.badge]][nuget]

[![][nuget.conventions.badge]][nuget.conventions]

[![][nuget.environment.settings.badge]][nuget.environment.settings]

[![][nuget.unit.badge]][nuget.unit]

</div>
</div>

## Overview

`Be.Stateless.BizTalk.Dsl.Binding` is part of the `BizTalk.Factory`'s [Development Packages](./../../../README.md#development-packages). This component provides an embedded `C#` DSL allowing the developer to define the bindings of Microsoft BizTalk Server® applications in a code-first type-safe way.

## Rationale

Deploying a Microsoft BizTalk Server® application in various environments is often a tedious and error prone task. One developer usually bootstraps the deployment process by first _manually_ deploying and configuring the application locally in order to be able to produce parameterized deployment artifacts such as `XML` bindings.

To this regard, [BizTalk Deployment Framework](https://github.com/BTDF/DeploymentFramework) provides a better and much more repeatable alternative thanks to its [Binding Files](http://www.tfabraham.com/BTDFDocs/V5_5/DeploymentFrameworkForBizTalkDocs.html?WorkingwithBindingsFiles.html), but the task is still tedious and error-prone, and the developer must still often bootstrap such a `Binding File` by exporting the bindings of the Microsoft BizTalk Server® application that he has _manually_ deployed locally beforehand.

Due to their deployment-time preprocessing for a given target environment, importing `XML` bindings may often fail for a variety of reasons. For instance, the generated `XML` bindings may be corrupted due to badly written preprocessing directives, invalid parameter values, or, because after all, `XML` bindings do contain lots of _magic_ strings &mdash;e.g. host instance names, assembly-qualified type names like maps, schemas, orchestrations, pipelines, pipeline components, and so on. Because their preprocessing happens at deployment-time, troubleshooting `XML` bindings import failures is often painful because it only fails when the Microsoft BizTalk Server® application is actually deployed in its target environment and not when the deployment package is produced &mdash;which typically occurs on the build server, that is to say, much sooner.

`BizTalk.Factory` departs from these repetitive, error-prone, and too often manual operations by allowing the developer to write the bindings of the Microsoft BizTalk Server® application he is currently developing right from the start in `C#` without any need to bootstrap the process in any way. Thanks to the embedded `C#` DSL offered by `Be.Stateless.BizTalk.Dsl.Binding`, the developer can configure all the various aspects of the bindings of a given Microsoft BizTalk Server® application for every target environment in which it is supposed to be deployed.

These `C#` code-first bindings will be used at deployment time to generate the `XML` bindings to be imported in Microsoft BizTalk Server® for the targeted environment. As we will see, these code-first bindings can &mdash;and should&mdash; be _unit_ tested during build, guaranteeing this way that the `XML` bindings can be generated and will successfully import in any target environment.

> **Remark** The only reason why `XML` bindings could still fail to import will be due to misalignment between the conventions used by the code and the ones used by the actual configuration of the Microsoft BizTalk Server® Group, like, for instance, host instance names.

## Basic Usage

> **Downloads** The code samples used in this user guide have been made available in the [Be.Stateless.BizTalk.Factory.Samples][github.samples] GitHub repository.

Let us imagine we are writing the bindings for the Microsoft BizTalk Server® `Accounting` application of a fictitious company called _Org.Anization_.

First of all, the developer has to create a new `.NET` class library project &mdash;let us call it `Org.Anization.Accounting.Bindings`&mdash; and reference the [Be.Stateless.BizTalk.Dsl.Binding][nuget] `NuGet` package. Being a seasoned developer, he will also create a second test project &mdash;let us call it `Org.Anization.Accounting.Bindings.Tests`&mdash; and reference the [Be.Stateless.BizTalk.Dsl.Binding.Unit][nuget.unit] `NuGet` package so as to be able to continuously test and validate the Microsoft BizTalk Server® application bindings for the `Accounting` application.

Now that we have created the bindings project, as well as the automated test project, we are ready to write the configuration for the various aspects of the Microsoft BizTalk Server® `Accounting` application. `Be.Stateless.BizTalk.Dsl.Binding` exposes and supports the following application binding aspects and allows the developer to configure them entirely in `C#`:

- [Applications](./Application.md),
- [Orchestrations](./Orchestration.md),
- [Receive Ports](./ReceivePort.md) and [Receive Locations](./ReceiveLocation.md),
- [Send Ports](./SendPort.md),
- [Pipelines](./Pipeline.md),
- [Transports](./Transport.md),
- [Adapters](./Adapter.md).

> **Remark** `Be.Stateless.BizTalk.Dsl.Binding` does not currently supports the `Send Port Groups` and the `Parties` &mdash;or `Role Links`&mdash; binding aspects.

## Advanced Usages

To better support the declaration of application bindings, the `Binding DSL` also offers a series of convenient and powerful features to effectively streamline and reduce the code one has to write:

- [Environment Dependent Values](./EnvironmentDependentValues.md)
- [Environment Overrides](./EnvironmentOverrides.md)
- [Naming Convention](./NamingConvention.md)
- [Host Resolution Policy](./HostResolutionPolicy.md)
- [`TimeSpan` Usage Generalization](./TimeSpanUsageGeneralization.md)

## Consuming Code-First Bindings

So far we have seen how to write Microsoft BizTalk Server® application bindings, at varying levels of refinement, by leveraging the features of `BizTalk.Factory`'s `Binding DSL`. It has also been said that the `C#` code-first bindings will be used at deployment time to generate the `XML` bindings to be imported in Microsoft BizTalk Server® for the targeted environment. Generating the `XML` bindings is just one of the many uses one could make of an application's `C#` code-first bindings, and `BizTalk.Factory` comes with several of them that we will cover later on.

But before that, it is worth mentioning that the [visitor pattern][visitor-pattern] is the key mechanism through which one can put these code-first application bindings to use. Thanks to the combined work of both [`IApplicationBindingVisitor`][i-application-binding-visitor] and [`IVisitable<TVisitor>`][i-visitable] interfaces together with the [VisitorPipeline][visitor-pipeline] class, it is actually quite easy to write a custom visitor to benefit from these code-first application bindings: one simply has to provide an implementation of the [`IApplicationBindingVisitor`][i-application-binding-visitor] interface.

Out of the box, `BizTalk.Factory`'s `Binding DSL` provides 3 implementations of the [`IApplicationBindingVisitor`][i-application-binding-visitor] interface:

- The [EnvironmentOverrideApplicator][environment-override-applicator] class, whose purpose is to ensure that the application bindings are all set for a given target deployment environment &mdash;in concrete terms it makes sure that the `ApplyEnvironmentOverrides` method has been called against all instances that make up the application binding object model, see [Environment Overrides](./EnvironmentOverrides.md);

- The [ApplicationBindingValidator][application-binding-validator] class, whose purpose is to check whether the application bindings are valid for one given target deployment environment &mdash;in concrete terms it makes sure that the `Validate` method has been called against all instances that make up the application binding object model;

- The [BindingInfoBuilder][binding-info-builder] class, whose purpose is to serialize to `XML` the application binding object model that has been set for a given target deployment environment.

Notice that though the [EnvironmentOverrideApplicator][environment-override-applicator] is an internal class &mdash;i.e. not accessible to the end-user,&mdash; it is nevertheless guaranteed to be called by the [VisitorPipeline][visitor-pipeline], whose purpose is precisely to make sure that all the environment overrides have been applied and the bindings validated before eventually calling any custom [`IApplicationBindingVisitor`][i-application-binding-visitor] implementation.

Finally, even though the [BindingInfoBuilder][binding-info-builder] class is bundled in the [Be.Stateless.BizTalk.Dsl.Binding][nuget] `NuGet` package, one has to install the [`BizTalk.Deployment`](../../../PowerShell/Module/BizTalk/Deployment/README.md) `PowerShell` module to actually be able to generate the `XML` bindings.

<!-- links -->

[doc.main]: https://www.stateless.be/ "BizTalk.Factory SDK"
[doc.this]: https://www.stateless.be/BizTalk/Dsl/Binding "Be.Stateless.BizTalk.Dsl.Binding"
[github]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding "Be.Stateless.BizTalk.Dsl.Binding GitHub Repository"
[github.badge]: https://img.shields.io/static/v1?label=Repository&message=Be.Stateless.BizTalk.Dsl.Binding&logo=github
[github.samples]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples
[nuget]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Dsl.Binding "Be.Stateless.BizTalk.Dsl.Binding NuGet Package"
[nuget.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Dsl.Binding.svg?label=Be.Stateless.BizTalk.Dsl.Binding&style=flat&logo=nuget
[nuget.conventions]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Dsl.Binding.Conventions
[nuget.conventions.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Dsl.Binding.Conventions.svg?label=Be.Stateless.BizTalk.Dsl.Binding.Conventions&style=flat&logo=nuget
[nuget.environment.settings]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Dsl.Environment.Settings
[nuget.environment.settings.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Dsl.Environment.Settings.svg?label=Be.Stateless.BizTalk.Dsl.Environment.Settings&style=flat&logo=nuget
[nuget.unit]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Dsl.Binding.Unit "Be.Stateless.BizTalk.Dsl.Binding.Unit NuGet Package"
[nuget.unit.badge]: https://img.shields.io/nuget/v/Be.Stateless.BizTalk.Dsl.Binding.Unit.svg?label=Be.Stateless.BizTalk.Dsl.Binding.Unit&style=flat&logo=nuget
[pipeline.ci]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=61&branchName=master "Azure DevOps Continuous Integration Build Pipeline"
[pipeline.ci.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Dsl.Binding%20Continuous%20Integration?branchName=master&label=Continuous%20Integration%20Build
[pipeline.mr]: https://dev.azure.com/icraftsoftware/be.stateless/_build/latest?definitionId=62&branchName=master "Azure DevOps Release Build Pipeline"
[pipeline.mr.badge]: https://dev.azure.com/icraftsoftware/be.stateless/_apis/build/status/Be.Stateless.BizTalk.Dsl.Binding%20Manual%20Release?branchName=master&label=Manual%20Release%20Build
[release]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/releases/latest "Be.Stateless.BizTalk.Dsl.Binding Release"
[release.badge]: https://img.shields.io/github/v/release/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding?label=Release&logo=github

<!--  -->

[application-binding-validator]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Visitor/ApplicationBindingValidator.cs
[binding-info-builder]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Visitor/BindingInfoBuilder.cs
[environment-override-applicator]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Visitor/EnvironmentOverrideApplicator.cs
[i-application-binding-visitor]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/IApplicationBindingVisitor.cs
[i-visitable]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Abstractions/blob/master/src/Be.Stateless.BizTalk.Dsl.Abstractions/Dsl/IVisitable.cs
[visitor-pattern]: https://en.wikipedia.org/wiki/Visitor_pattern
[visitor-pipeline]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Visitor/Pipeline/VisitorPipeline.cs

<!--
cSpell:ignore anization
-->
