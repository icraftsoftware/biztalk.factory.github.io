# Environment Dependent Values

> **Downloads** The code samples used in this user guide have been made available in the [Be.Stateless.BizTalk.Factory.Samples][github.samples] GitHub repository.

Having different configuration property values with each target deployment environment is a typical deployment scenario, which is usually achieved through configuration files that vary between environments. The equivalent of the Microsoft BizTalk Server® configuration file is its management database, which is populated primarily when importing `XML` bindings. As we have seen, the `XML` bindings to be imported during deployment are generated based on the `C#` code-first bindings written with the `Binding DSL` configuration API of `BizTalk.Factory`.

Instead of having different configuration files we need to produce `XML` binding files according to their target deployment environments. To support this simple scenario, `BizTalk.Factory`'s `Binding DSL` provides three static helper classes that interact with ech other:

- A [DeploymentContext][deployment-context], that provides a read-only &mdash;actually, settable via unit testing helper classes or `PowerShell` deployment commands&mdash; `string` property, `TargetEnvironment`, that denotes the environment for which the `XML` bindings are currently being generated.

- A [TargetEnvironment][target-environment] class that provides a predefined list of target environments **ordered** according to their maturity level &mdash;i.e. `DEVELOPMENT` = "DEV", `BUILD` = "BLD", `INTEGRATION` = "INT", `ACCEPTANCE` = "ACC", `PREPRODUCTION` = "PRE", and `PRODUCTION` = "PRD",&mdash; and few predicate extension methods helping to determine the current target deployment environment or a minimum one, allowing the developer to write code as follows:

  ```csharp
  using Be.Stateless.BizTalk.Install;

  // true if DeploymentContext.TargetEnvironment is "PRD"
  if (DeploymentContext.TargetEnvironment.IsProduction()) {
     ...
  }

  // true if DeploymentContext.TargetEnvironment is "ACC" or "PRE" or "PRD"
  if (DeploymentContext.TargetEnvironment.IsAcceptanceUpwards()) {
     ...
  }
  ```

- [EnvironmentDependentValue][environment-dependent-value] provides strongly typed extensions methods ensuring that, for a given configuration property, a value, of the correct type, is defined for each target environment; allowing the developer to write code as follows:

  ```csharp
  using Be.Stateless.BizTalk.Install;

  public static class Settings
  {
     public static DateTime DateProperty => EnvironmentDependentValue
  		.ForDevelopment(new DateTime(2021, 3, 3))
  		.ForAcceptanceUpwards(DateTime.MinValue);

  	public static int IntegerProperty => EnvironmentDependentValue
  		.ForAcceptance(1)
  		.ForBuild(2)
  		.ForDevelopment(3)
  		.ForPreProduction(4)
  		.ForProduction(5);

  	public static string StringProperty => EnvironmentDependentValue
  		.ForDevelopmentOrBuild("one.1")
  		.ForAcceptance("one.2")
  		.ForPreProductionUpwards("one.3");
  }
  ```

  Recall that we have an automated test that validates that the `XML` bindings can be generated for all the target deployment environments that concern us. This test now fails throwing a couple of `NotSupportedException`s saying that _'DateProperty' does not provide a value for target environment 'BLD'_ and _'DateProperty' does not provide a value for target environment 'INT'_, therefore ensuring that the developer does not forget to define them.

> **Remark** The developer is obviously free to define his own custom list of target environments, but then he would have to redefine his own equivalent of the `TargetEnvironment` and `EnvironmentDependentValue` classes.

<!-- links -->

[github.samples]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples

<!--  -->

[deployment-context]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Environment.Settings/Install/DeploymentContext.cs
[environment-dependent-value]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Environment.Settings/Install/EnvironmentDependentValue.cs
[target-environment]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Environment.Settings/Install/TargetEnvironment.cs

<!--
cSpell:ignore PREPRODUCTION
-->
