# Application Binding

> **Downloads** The code samples used in this user guide have been made available in the [Be.Stateless.BizTalk.Factory.Samples][github.samples] GitHub repository.

Unsurprisingly, the developer has to start with the [ApplicationBinding][application-binding] object when willing to write the bindings of a Microsoft BizTalk Server® application. Let us follow along and start writing code in the `Org.Anization.Accounting.Bindings` and `Org.Anization.Accounting.Bindings.Tests` projects we just created.

Let us create the following `Application` class in the `Org.Anization.Accounting.Bindings` project. This application binding is for an empty Microsoft BizTalk Server® application, that is to say an application without any of the Microsoft BizTalk Server® artifacts that `Be.Stateless.BizTalk.Dsl.Binding` supports &mdash;i.e. orchestrations, send ports, receive ports, and receive locations.

```csharp
using Be.Stateless.BizTalk.Dsl.Binding;

namespace Org.Anization.Accounting
{
  public class Application : ApplicationBinding
  {
    public Application()
    {
      Name = "Accounting";
      Description = "Org.Anization's BizTalk Server Accounting Application";
    }
  }
}
```

To allow for continuous testing and validation of the `Accounting` application bindings, let us create the following `ApplicationFixture` in the `Org.Anization.Accounting.Bindings.Tests` project.

```csharp
using Be.Stateless.BizTalk.Install;
using Be.Stateless.BizTalk.Unit.Dsl.Binding;
using FluentAssertions;
using Xunit;
using static FluentAssertions.FluentActions;

namespace Org.Anization.Accounting
{
  public class ApplicationFixture : ApplicationBindingFixture<Application>
  {
    [Theory]
    [InlineData(TargetEnvironment.DEVELOPMENT)]
    [InlineData(TargetEnvironment.BUILD)]
    [InlineData(TargetEnvironment.ACCEPTANCE)]
    [InlineData(TargetEnvironment.PRODUCTION)]
    public void GenerateApplicationBinding(string targetEnvironment)
    {
      Invoking(() => GenerateApplicationBindingForTargetEnvironment(targetEnvironment))
        .Should().NotThrow();
    }
  }
}
```

Thanks to this fixture, the whole `Accounting` application bindings would be generated and validated in memory every time the unit tests would be run for every target environment where the `Accounting` application is supposed to be deployed.

> **Remark** `BizTalk.Factory` defines a bunch of target environment names in the [Be.Stateless.BizTalk.Install.TargetEnvironment][target-environment] class, available in the `Be.Stateless.BizTalk.Dsl.Environment.Settings` `NuGet` package.

Notice that if the developer wishes to generate the `XML` bindings files on disk, he could write the following code, which would produce a file for each target environment every time the unit tests are run:

```csharp
using System.IO;
using System.Runtime.CompilerServices;
using System.Text;
using Be.Stateless.BizTalk.Install;
using Be.Stateless.BizTalk.Unit.Dsl.Binding;
using Xunit;

namespace Org.Anization.Accounting
{
  public class ApplicationFixture : ApplicationBindingFixture<Application>
  {
    [Theory]
    [InlineData(TargetEnvironment.DEVELOPMENT)]
    [InlineData(TargetEnvironment.BUILD)]
    [InlineData(TargetEnvironment.ACCEPTANCE)]
    [InlineData(TargetEnvironment.PRODUCTION)]
    public void GenerateApplicationBindingFile(string targetEnvironment)
    {
      var path = Path.Combine(
        GetRepoRootPath(),
        $"Org.Anization.Accounting.{targetEnvironment}.bindings.xml"
      );
      File.WriteAllText(
        path,
        GenerateApplicationBindingForTargetEnvironment(targetEnvironment),
        Encoding.Unicode);
    }

    private string GetRepoRootPath([CallerFilePath] string sourceFilePath = "")
    {
      return Path.GetFullPath(Path.Combine(Path.GetDirectoryName(sourceFilePath)!, @"..\..\"));
    }
  }
}
```

Out of curiosity, the `XML` bindings file corresponding to the previous sample would look like this &mdash;though not very interesting nor useful:

```xml
<BindingInfo xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" Assembly="Microsoft.BizTalk.Deployment, Version=3.0.1.0, Culture=neutral, PublicKeyToken=31bf3856ad364e35" Version="3.5.1.0" BindingStatus="NoBindings" BoundEndpoints="0" TotalEndpoints="0">
  <Description>Org.Anization's BizTalk Server Accounting Application</Description>
  <Timestamp>2021-12-08T15:10:04.9700713+01:00</Timestamp>
  <ModuleRefCollection>
    <ModuleRef Name="[Application:Accounting]" Version="" Culture="" PublicKeyToken="" FullName="[Application:Accounting], Version=, Culture=, PublicKeyToken=">
      <Services />
      <TrackedSchemas />
    </ModuleRef>
  </ModuleRefCollection>
  <SendPortCollection />
  <DistributionListCollection />
  <ReceivePortCollection />
  <PartyCollection xsi:nil="true" />
</BindingInfo>
```

Let us now have a look at how as a developer we can configure the [Receive Ports](./ReceivePort.md), [Receive Locations](./ReceiveLocation.md), and [Send Ports](./SendPort.md).

<!-- links -->

[application-binding]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/ApplicationBinding.cs
[github.samples]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples
[target-environment]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Environment.Settings/Install/TargetEnvironment.cs

<!--
cSpell:ignore Anization Xunit
-->
